---
type: paper
title: "Do-PFN: In-Context Learning for Causal Effect Estimation"
authors: ""
year: 2025
venue: ""
url: ""
topics: [causality]
tags: [pfn, causal-foundation-model, cate]
status: read
date: 2025-10-29
builds_on: []
my_rating:
source_post: https://letter-night.tistory.com/1079
migration: summary
migrated: 2026-11-23
---

# Do-PFN: In-Context Learning for Causal Effect Estimation

**기존 글**
- [[Do-PFN] In-Context Learning for Causal Effect Estimation](https://letter-night.tistory.com/1079) (2025-10-29)

## 한 줄 요약

## 핵심 내용

## 나의 리뷰
*(2025-10-29 글 "예상대로 흥미진진한데"에서 옮김)*
- 기대했던 만큼 흥미롭다. Appendix는 아직 못 읽어 실험 세부사항은 모른다.
- CATE 추정에 쓸 ML 방법이 Do-PFN 말고는 없었나? baseline을 더 다양하게 비교했으면 좋겠다.
- 여러 dataset으로 코드를 직접 돌려 볼 계획.
- causal effect estimation은 검증할 수 없는 assumption에 기대므로 sensitivity analysis 같은 robustness check가 반드시 필요하다.
- assumption을 완화했다는 점은 큰 장점이고, unidentifiable한 상황에서도 어느 정도 추론이 가능하다는 데 의의가 있다.
- 다만 assumption이 위반되었을 때 성능이 얼마나 떨어지는지 확인이 필요하다.
- unidentifiable한 상황의 uncertainty를 sensitivity analysis처럼 정량화해 준다면, 의료·제약 같은 critical한 상황에서도 쓸모 있는 foundation model이 될 것이다.

## 열린 질문 / 한계

## 연결

## 에이전트 노트
