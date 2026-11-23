---
type: thought
title: "causal inference를 공부하며 3탄: 참고서 비교와 LLM/Agent의 역할"
topics: [causality]
tags: [textbook, agent-for-causal-inference, assumptions]
date: 2026-11-08
source_post: https://letter-night.tistory.com/1510
migration: summary
migrated: 2026-11-23
---

# causal inference를 공부하며 3탄: 참고서 비교와 LLM/Agent의 역할

> 기존 블로그 글에서 옮긴 요약입니다. 원문 표현을 최대한 살렸지만 전문은 아닙니다.
- [causal inference 를 공부하며 3탄](https://letter-night.tistory.com/1510) (2026-11-08)

## 나의 생각
- *What If*를 처음부터 차례로 읽는 중이다. 진지하게 연구하려는 사람에게 **필독서**다.
- 입문 때 본 세 참고서도 모두 추천한다.
  - Peng Ding 강의노트 (*A First Course in Causal Inference*)
  - Brady Neal 강의노트
  - *Causal Inference for the Brave and True*: 경제학 관점이라 DiD, Synthetic Control, Conformal inference 설명이 쉽고 자세하다. 다만 수학적 엄밀성을 원할 때는 아쉬울 수 있다.
- *What If*는 causal question, intervention, potential outcome을 명시하고, DAG에서 출발해 exchangeability, positivity, consistency를 정의한다. time-varying treatment까지 다루며, 다른 책에서 생략된 **행간을 채워준다**.
  - bias를 confounding, selection, measurement, random variability로 나누어 분석하고, 검증 불가능한 가정에 대한 비판과 대응 방안을 제시한다.
- **문제의식:** causal inference는 expert knowledge와 합의된 가정에 의존한다. 가정이 틀리면 추론의 정당성이 사라지는데, 가정에 대한 민감도를 제시하기도 어렵다.
- **제안: LLM/Agent 기반 causal inference**
  - 방대한 지식으로 DAG·SCM 구조를 찾고 추론 오류를 찾아낸다
  - backdoor 기준을 만족하면서 새로운 bias를 유발하지 않는 covariate를 탐색한다
  - 새로운 가설을 제시한다
  - 단일 point estimate 대신 여러 시나리오와 불확실성을 제시한다
  - 특히 **multimodality를 활용한 causal inference**에 관심이 있다

## 질문
-

## 연결된 자료

- [★ 고전의 중요성 ★](2026-11-09-importance-of-classics.md)
- [[부치지 못한 편지 2] Causal effect under time-varying treatment](2026-11-05-causal-effect-under-time-varying-treatment.md)

## 에이전트 노트
