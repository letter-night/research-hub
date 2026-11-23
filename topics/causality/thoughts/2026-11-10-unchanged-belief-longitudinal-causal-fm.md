---
type: thought
title: "여전한 믿음: 시계열 인과추론 foundation model"
topics: [causality]
tags: [time-varying-treatment, causal-foundation-model, multimodal, medical]
date: 2026-11-10
source_post: https://letter-night.tistory.com/1512
migration: summary
migrated: 2026-11-23
---

# 여전한 믿음: 시계열 인과추론 foundation model

> 기존 블로그 글에서 옮긴 요약입니다. 원문 표현을 최대한 살렸지만 전문은 아닙니다.
- [여전한 믿음 ㅎㅎ](https://letter-night.tistory.com/1512) (2026-11-10)

## 나의 생각
- 시계열 인과추론(causal inference foundation model for longitudinal data) 연구는 결과를 내지 못하고 실패했지만, 방향에 대한 믿음은 변하지 않았다.
- 기존 causal effect estimation foundation model은 **굉장히 초기단계**다. 더 복잡한 DAG 구조와 다양한 modality를 통합해 추론하는 모델이 나올 여지가 크다.
- 실세계 인과 문제는 time-fixed가 아니다. 환자 trajectory를 따라가는 time-varying effect를 고려해야 하며, 이를 무시한 1회성 estimation은 meaningless하다.
- 표 형태의 covariate뿐 아니라 MRI 같은 영상 modality도 함께 고려하는 것이 더 현실적이다.
- 다양한 시나리오를 고려해 potential bias 하의 uncertainty를 함께 제시하고, 추론 과정을 DAG와 함께 transparent하고 interpretable하게 보여주는 모델이 필요하다.
- 궁극적으로 **multi-modal time-varying causal effect estimation foundation model (Agent)** 이 나오기를 기대한다.

## 질문
-

## 연결된 자료

- [[부치지 못한 편지 2] Causal effect under time-varying treatment](2026-11-05-causal-effect-under-time-varying-treatment.md)
- [★ 고전의 중요성 ★](2026-11-09-importance-of-classics.md)

## 에이전트 노트
