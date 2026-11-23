---
type: thought
title: "[부치지 못한 편지 2] Causal effect under time-varying treatment"
topics: [causality]
tags: [time-varying-treatment, medical, neural-de]
date: 2026-11-05
source_post: https://letter-night.tistory.com/1508
migration: summary
migrated: 2026-11-23
---

# [부치지 못한 편지 2] Causal effect under time-varying treatment

> 기존 블로그 글에서 옮긴 요약입니다. 원문 표현을 최대한 살렸지만 전문은 아닙니다.
- [[부치지 못한 편지 2] Causal effect under time-varying treatment](https://letter-night.tistory.com/1508) (2026-11-05)

## 나의 생각
- Causal inference가 가장 critical하게 쓰이는 분야는 medical domain이다. treatment에 따른 환자 건강 상태 추정은 의료인의 decision making에 guidance가 된다.
- 질문: **time-fixed 상황에서 DAG와 SCM으로 추론한 결과가 얼마나 유효할까?**
  - time-dimension을 고려하지 않은 추론은 실제 인과효과의 일부만 본다. 극단적으로 말하자면 meaningless할 수도 있다.
- 환자의 상태(time-varying covariates)와 treatment는 시간에 따라 변하고, treatment 시점도 개인마다 다르다. 이런 dynamics를 다루려면 **Neural Differential Equation 기반 모델링**이 가장 적절해 보인다.
- 아쉬움: time-varying treatment 하의 causal inference에서 제대로 된 연구 결과를 내지 못했다.
- 이후 알게 된 것: time-varying treatment 상황에서는 time-varying confounder 조정뿐 아니라 **과거 treatment history**도 고려해야 한다. time-fixed 상황에서 현재 treatment 효과만 측정하더라도, 과거 treatment 기록을 무시하면 bias가 생긴다.

## 질문
-

## 연결된 자료
- *Continuous-Time Modeling of Counterfactual Outcomes Using Neural CDEs* 및 후속 논문들
- Hernán & Robins, *What If* (time-varying treatment의 g-computation)
- [여전한 믿음 ㅎㅎ](2026-11-10-unchanged-belief-longitudinal-causal-fm.md)
- Continuous-Time Modeling of Counterfactual Outcomes Using Neural CDEs — https://letter-night.tistory.com/1195

## 에이전트 노트
