---
type: idea
id: I04
title: "Multimodal time-varying causal effect estimation foundation model (Agent)"
topics: [causality, agentic-ai]
status: parked
proposed_by: me
origin: [1512, 1508, 1511, 1195, 1196, 1227]
date: 2026-01-19
updated: 2026-11-23
---

# I04. Multimodal time-varying causal effect estimation foundation model (Agent)

**출발점이 된 기록**
- [여전한 믿음 ㅎㅎ](../topics/causality/thoughts/2026-11-10-unchanged-belief-longitudinal-causal-fm.md)
- [[부치지 못한 편지 2] Causal effect under time-varying treatment](../topics/causality/thoughts/2026-11-05-causal-effect-under-time-varying-treatment.md)
- [★ 고전의 중요성 ★](../topics/causality/thoughts/2026-11-09-importance-of-classics.md)
- [Continuous-Time Modeling of Counterfactual Outcomes Using Neural CDEs](../topics/causality/papers/2022-te-cde.md)
- [[BNCDE] Bayesian Neural CDEs for Treatment Effect Estimation](../topics/causality/papers/2024-bncde.md)
- [[SCIP-Net] Stabilized Neural Prediction of Potential Outcomes in Continuous Time](../topics/causality/papers/2025-scip-net.md)

## 질문
환자 trajectory를 따라가며 시변 처치효과를 추정하고, 표 형태 covariate와 영상(MRI 등)을 함께 쓰며, potential bias 하의 불확실성과 DAG를 함께 제시하는 foundation model(또는 agent)을 만들 수 있는가?

## 배경
- 이전에 시도한 longitudinal causal FM 연구는 결과를 내지 못했다 (2026-11 회고). 그래도 방향에 대한 믿음은 그대로.
- 기존 causal effect FM은 time-fixed, 단일 modality, 단순 DAG에 머물러 있다.

## 배운 점 (기록에서)
- 시변 confounder 조정뿐 아니라 **과거 treatment history**를 무시하면 time-fixed 효과 추정도 편향된다.
- 연속 시간 dynamics에는 Neural CDE 계열이 적절해 보였다 (TE-CDE → BNCDE → SCIP-Net).

## 다시 꺼낼 조건
- 문제를 쪼갤 것: (a) 시변 처치 PFN (합성 prior를 시계열 SCM으로 확장) → (b) 불확실성 → (c) multimodal. 한 번에 다 하지 않기.

## 에이전트 노트
- **[2026-11-23 · Management]** 기존 블로그 기록에서 추출해 아이디어로 정리했습니다. 문장은 연구자의 글에서 가져왔고, "접근 방법 후보"와 "다음 한 걸음"의 일부는 에이전트가 정리한 것입니다.
