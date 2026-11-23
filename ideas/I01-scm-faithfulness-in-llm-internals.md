---
type: idea
id: I01
title: "LLM 내부는 프롬프트의 인과 그래프를 충실하게 구현하는가 (SCM faithfulness)"
topics: [mech-interp, causality]
status: draft
proposed_by: me
origin: [1360, 1361, 1190, 1187, 1371, 1423]
date: 2026-01-09
updated: 2026-11-23
---

# I01. LLM 내부는 프롬프트의 인과 그래프를 충실하게 구현하는가 (SCM faithfulness)

**출발점이 된 기록**
- [[on-going (until next week)] research question](https://letter-night.tistory.com/1360)
- [[Draft] Testing SCM Faithfulness in LLM Internals](https://letter-night.tistory.com/1361)
- [그렇다면 Mechanistic Interpretability는 LLM이 causal reasoning을 할 수 있다는 증거 아닌감?](../topics/mech-interp/thoughts/2026-01-12-is-mi-evidence-of-causal-reasoning.md)
- [!! Mechanistic Interpretability가 Causal Representation & discovery에 답을 주었다!!](../topics/mech-interp/thoughts/2026-01-09-mi-answers-causal-representation.md)
- [생성모델 관점에서 생각해보더라도](../topics/mech-interp/thoughts/2026-06-15-generative-model-view-of-mi.md)
- [그간의 생각 정리, 근데 너무 어려움](../topics/mech-interp/thoughts/2026-07-26-research-process-proposal-is-hard.md)

## 질문
> Do LLMs internally implement the causal graph described in a prompt, or do they answer causal questions using surface-level correlations?

알려진 인과 그래프 $G$가 있는 과제에서, 인과 변수 $X_i$에 대응하는 내부 feature $z_i$를 찾을 수 있는가? 그리고 $do(z_i)$ 개입이 $G$가 예측하는 대로 하위 출력 $Y$를 바꾸는가?

## 왜 중요한가
- 기존 연구는 인과성으로 **모델 행동을 설명**하는 데 집중했다. 이 아이디어는 MI로 **모델의 인과 추론 자체**를 들여다본다.
- "LLM이 data generating mechanism을 이해하는가"라는 Big Question에 대한 가장 직접적인 검증 방법이다.

## 가설
프롬프트에 기술된 SCM의 변수에 대응하는 내부 feature를 식별할 수 있고, 그 feature에 개입하면 SCM의 do-개입 예측과 일치하는 activation·출력 변화가 나타난다. 이는 paraphrase, 변수 이름 바꾸기, OOD 그래프 구조에서도 유지되며, collider·confounder 사례에서는 예측 가능한 방식으로 실패한다.

## 접근 방법 후보
- Linear probe로 causal variable 값 복원
- SAE / transcoder로 해석 가능한 feature 탐색
- Activation patching, interchange intervention으로 인과적 사용과 변수 정렬 검증 (causal abstraction 프레임)
- 개입을 통한 feature-level 그래프 복원 → gold DAG와 비교

## 실험 설계 (초안, 2026-06-10)
- 변수 3–8개의 합성 SCM. 변수 이름과 그래프 구조를 무작위화하고 관측·개입 질의를 통제
- 소형 open-weight 모델에서 시작 → instruction-tuned 모델로 확장
- **핵심 통제:** 관측 분포는 같고 개입 분포만 다른 그래프 쌍. 상관에 의존하면 구별하지 못해야 하고, SCM을 표현하면 구별해야 한다
- 오해를 부르는 변수명 vs 추상 변수명 → 사전지식 의존 여부 확인
- 지표: answer accuracy, interventional/counterfactual accuracy, interchange intervention accuracy, 복원 그래프와 gold DAG 간 SHD, $|\widehat{\mathrm{ATE}}-\mathrm{ATE}|$, OOD 일반화

## 알려진 관련 연구 / 공백
- Sparse Feature Circuits — https://openreview.net/forum?id=I4e82CIDxv
- Causal Abstraction: A Theoretical Foundation for Mechanistic Interpretability — https://www.jmlr.org/papers/volume26/23-0058/23-0058.pdf
- Interpretability at Scale: Identifying Causal Mechanisms in Alpaca (NeurIPS 2023)
- Causal Reasoning and Large Language Models: Opening a New Frontier for Causality — https://openreview.net/forum?id=mqoxLkX210
- Can Large Language Models Infer Causation from Correlation? — https://arxiv.org/abs/2306.05836
- CausalBench — https://arxiv.org/abs/2404.06349
- Causal Inference with Large Language Model: A Survey — https://aclanthology.org/2025.findings-naacl.327.pdf

## 실행 가능성
- 합성 SCM + 소형 모델이면 단일 GPU로 시작 가능. Neuronpedia / circuit-tracer로 attribution graph를 먼저 만들어 보는 것이 첫 실험.

## 다음 한 걸음
- (2026-07-26 메모) high-level에선 가능해 보이지만 세부가 어렵다 → 변수 3개짜리 chain/fork/collider 세 그래프로 **최소 실험** 하나를 정의하기.

## 에이전트 노트
- **[2026-11-23 · Management]** 기존 블로그 기록에서 추출해 아이디어로 정리했습니다. 문장은 연구자의 글에서 가져왔고, "접근 방법 후보"와 "다음 한 걸음"의 일부는 에이전트가 정리한 것입니다.
- **[2026-11-23 · Research]** 2026년에 나온 가까운 연구들입니다. 차별점을 정할 때 먼저 읽어 보세요.
  - *Belief or Circuitry? Causal Evidence for In-Context Graph Learning* (arXiv 2605.08405, 2026-05): in-context로 주어진 그래프 구조가 residual stream에 표현되고, activation patching과 steering으로 인과적으로 개입함. 방법론이 I01과 가장 가깝습니다. https://arxiv.org/abs/2605.08405
  - *My Graph Doesn't Help! Analyzing Causal Graph Construction, Representation, and Utility in LLMs* (NeurIPS 2026): 그래프를 충실하게 복원하는 능력과 그것을 추론에 쓰는 능력이 서로 다르다는 행동 수준 결과. I01의 "표현 vs 사용" 구분에 근거가 됩니다. https://neurips.cc/virtual/2026/162002
  - *CausalPrism* (EMNLP 2026 Findings): 개입 기반 인과 추론을 구성 요소별로 평가하는 프레임워크. 행동 평가 쪽 벤치마크 후보. https://aclanthology.org/2026.findings-emnlp.1294.pdf
  - *MIB: A Mechanistic Interpretability Benchmark* — causal variable localization 트랙이 interchange intervention 기반 평가를 제공합니다. https://arxiv.org/abs/2504.13151
  - *CLEAR: Can Language Models Really Understand Causal Graphs?* (2024): 행동 수준 인과 그래프 이해 벤치마크. https://arxiv.org/abs/2406.16605
- **[2026-11-23 · Advisor]** 차별점 후보: 위 연구들은 (a) 그래프 위상 자체의 표현, 또는 (b) 행동 수준 평가에 머뭅니다. I01의 고유한 기여는 **"관측 분포는 같고 개입 분포만 다른 그래프 쌍"** 통제입니다. 이 통제 하나로 상관 의존과 SCM 표현을 가를 수 있다는 점을 연구의 중심 주장으로 세우는 것을 권합니다.

