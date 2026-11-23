---
type: idea
id: I03
title: "In-context learning만으로 복잡한 DAG 구조를 추론할 수 있는가"
topics: [causality, mech-interp]
status: seed
proposed_by: me
origin: [1177, 1176, 1170]
date: 2026-01-04
updated: 2026-11-23
---

# I03. In-context learning만으로 복잡한 DAG 구조를 추론할 수 있는가

**출발점이 된 기록**
- [복잡한 DAG-structure로 in-context learning 하면..?](../topics/causality/thoughts/2026-01-06-complex-dag-in-context-learning.md)
- [Why induction head in Transformer is important for meta-learning?](../topics/mech-interp/concepts/induction-heads-and-meta-learning.md)
- [[COCONUT] Training LLMs to Reason in a Continuous Latent Space](../topics/agentic-ai/papers/2024-coconut.md)

## 질문
induction head가 meta-learning을 가능하게 한다면, PFN을 scaling up해서 **복잡한 DAG 구조를 추론하도록 in-context learning**을 시키면 어떻게 될까? COCONUT이 latent reasoning으로 복잡한 그래프 탐색을 한 것처럼, ICL만으로도 가능할까?

## 접근 방법 후보
- 그래프 크기·밀도를 늘려가며 PFN 계열 모델의 구조 복원 성능이 어디서 무너지는지 측정 (scaling curve)
- I02와 결합: 무너지는 지점에서 내부 표현이 어떻게 달라지는지

## 다음 한 걸음
- 합성 prior의 그래프 크기 분포가 논문마다 어떻게 설정되어 있는지 정리

## 에이전트 노트
- **[2026-11-23 · Management]** 기존 블로그 기록에서 추출해 아이디어로 정리했습니다. 문장은 연구자의 글에서 가져왔고, "접근 방법 후보"와 "다음 한 걸음"의 일부는 에이전트가 정리한 것입니다.
