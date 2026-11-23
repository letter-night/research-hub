---
type: idea
id: I02
title: "PFN 기반 인과 foundation model은 정말 내부에서 인과 그래프를 찾는가"
topics: [causality, mech-interp]
status: seed
proposed_by: me
origin: [1192, 1079, 1189, 1193]
date: 2025-10-29
updated: 2026-11-23
---

# I02. PFN 기반 인과 foundation model은 정말 내부에서 인과 그래프를 찾는가

**출발점이 된 기록**
- [정말로 implicit하게 causal graph를 찾고, 추론하였을까?](../topics/causality/thoughts/2026-01-14-did-pfn-find-causal-graph-implicitly.md)
- [[Do-PFN] In-Context Learning for Causal Effect Estimation](../topics/causality/papers/2025-do-pfn.md)
- [[CausalPFN] Amortized Causal Effect Estimation via In-Context Learning](../topics/causality/papers/2025-causalpfn.md)
- [[CausalFM] Foundation Models for Causal Inference via PFNs](../topics/causality/papers/2025-causalfm.md)

## 질문
Do-PFN, CausalPFN, CausalFM은 ground-truth 그래프 없이 관측 데이터만으로 causal effect를 추정한다. 논문은 이를 "implicit하게 causal graph를 찾고 추론한 결과"라고 설명한다. **MI로 모델 내부를 보면 실제로 그래프(또는 adjustment set)를 표현하고 있는가?**

## 왜 중요한가
- PFN은 합성 SCM prior로 학습되므로 **정답 그래프를 아는 상태에서 내부를 분석**할 수 있다. LLM보다 훨씬 통제된 실험대다.
- I01(LLM)과 같은 질문을 더 작은 모델에서 먼저 검증할 수 있다.

## 접근 방법 후보
- 공개된 PFN 체크포인트에 linear probe: 입력 데이터셋의 인접행렬, confounder 여부, adjustment set을 복원할 수 있는가
- 같은 관측 분포 / 다른 그래프 쌍으로 activation 비교
- 그래프 정보를 담은 방향에 개입했을 때 추정치가 바뀌는가

## 다음 한 걸음
- 어떤 PFN 계열 모델의 가중치가 공개되어 있는지 확인 (Research 에이전트)

## 에이전트 노트
- **[2026-11-23 · Management]** 기존 블로그 기록에서 추출해 아이디어로 정리했습니다. 문장은 연구자의 글에서 가져왔고, "접근 방법 후보"와 "다음 한 걸음"의 일부는 에이전트가 정리한 것입니다.
- **[2026-11-23 · Research]** 이 질문은 TabPFN에 대해서는 이미 연구가 나오고 있습니다.
  - *Does TabPFN Understand Causal Structures?* (Swelam et al., arXiv 2511.07236, 2025-11): TabPFN v2의 frozen embedding에서 adapter로 인접행렬을 복원했고, 인과 정보가 중간 layer에 모여 있음. https://arxiv.org/abs/2511.07236
  - *TabPFN Through The Looking Glass* (arXiv 2601.08181, 2026-01): 알려진 함수 구조를 가진 합성 과제로 TabPFN v2 내부를 probing. https://arxiv.org/abs/2601.08181
  - *Causal graph fusion across incomplete cohorts and causal steering of tabular foundation models* (arXiv 2611.09400): 정답 그래프가 있는 합성 SCM으로 TabPFN v2의 attention을 분석하고, 특정 layer에서 직접 원인에 대한 신호가 나타난다고 보고. https://arxiv.org/abs/2611.09400
- **[2026-11-23 · Advisor]** 이 연구들은 **예측 모델(TabPFN)이 그래프를 담고 있는가**를 봅니다. 아직 비어 있어 보이는 곳은 **효과 추정 모델(Do-PFN, CausalPFN, CausalFM)이 adjustment set이나 confounder 여부를 표현하고 실제로 쓰는가**입니다. 질문을 "그래프를 아는가"에서 "식별 전략을 구현하는가"로 좁히면 겹치지 않습니다. 상태를 `seed` → `exploring`으로 올릴 만합니다.

