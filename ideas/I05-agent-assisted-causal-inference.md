---
type: idea
id: I05
title: "Agent가 돕는 인과추론: DAG 탐색과 sensitivity analysis"
topics: [causality, agentic-ai]
status: seed
proposed_by: me
origin: [1511, 1510, 1078, 1151]
date: 2025-10-29
updated: 2026-11-23
---

# I05. Agent가 돕는 인과추론: DAG 탐색과 sensitivity analysis

**출발점이 된 기록**
- [★ 고전의 중요성 ★](../topics/causality/thoughts/2026-11-09-importance-of-classics.md)
- [causal inference 를 공부하며 3탄](../topics/causality/thoughts/2026-11-08-studying-causal-inference-3.md)
- [예상대로 흥미진진한데 → Do-PFN 노트의 나의 리뷰](../topics/causality/papers/2025-do-pfn.md)
- [여전히 풀리지 않은 숙제](../topics/causality/thoughts/2025-12-22-still-unsolved-homework.md)

## 질문
인과추론은 expert knowledge와 검증 불가능한 가정에 기대고, 가정이 틀렸을 때의 민감도를 제시하기 어렵다. **LLM/Agent가 (1) DAG를 제안·검증하고, (2) 여러 대안 그래프와 가정 위반 시나리오를 돌려 bias 범위를 정량화하고, (3) multimodal 정보를 활용**할 수 있는가?

## 왜 중요한가
- 모든 인과분석에 DAG와 sensitivity analysis가 함께 제시되어야 한다는 것이 나의 입장.
- Do-PFN류 모델의 약점(가정 위반 시 성능, unidentifiable 상황의 불확실성)을 agent 수준에서 보완할 수 있다.

## 접근 방법 후보
- Agent 파이프라인: 변수 설명 → 후보 DAG 여러 개 → 각 DAG의 adjustment set → 추정 → 그래프 간 추정치 분산을 불확실성으로 보고
- backdoor를 만족하면서 새 bias를 만들지 않는 covariate 탐색 (collider, M-bias 회피)
- 평가: 정답 그래프가 있는 반합성 벤치마크

## 다음 한 걸음
- LLM 기반 causal discovery / DAG 제안 연구 현황 조사 (Research 에이전트)

## 에이전트 노트
- **[2026-11-23 · Management]** 기존 블로그 기록에서 추출해 아이디어로 정리했습니다. 문장은 연구자의 글에서 가져왔고, "접근 방법 후보"와 "다음 한 걸음"의 일부는 에이전트가 정리한 것입니다.
