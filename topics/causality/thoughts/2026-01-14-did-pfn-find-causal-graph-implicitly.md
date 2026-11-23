---
type: thought
title: "정말로 implicit하게 causal graph를 찾고 추론했을까?"
topics: [causality, mech-interp]
tags: [pfn, causal-foundation-model, mech-interp]
date: 2026-01-14
source_post: https://letter-night.tistory.com/1192
migration: summary
migrated: 2026-11-23
---

# 정말로 implicit하게 causal graph를 찾고 추론했을까?

> 기존 블로그 글에서 옮긴 요약입니다. 원문 표현을 최대한 살렸지만 전문은 아닙니다.
- [정말로 implicit하게 causal graph를 찾고, 추론하였을까?](https://letter-night.tistory.com/1192) (2026-01-14)

## 나의 생각
- PFN 기반 causal inference foundation model(Do-PFN, CausalPFN, CausalFM)은 ground-truth causal graph를 모르는 상태에서 observational data만으로 causal inference를 수행한다.
- Do-PFN 논문은 이를 implicit하게 causal graph를 찾고 inference를 수행한 결과라고 주장한다.
- 질문: **이 모델들의 추론 과정에 mechanistic interpretability를 적용하면, 모델 내부에서 실제로 causal graph를 찾고 그 결과로 추론했음을 증명할 수 있을까?**
- 직접 해보고 싶다. 그런데 이거 어떻게 해야 하지?

## 질문
-

## 연결된 자료

- [Do-PFN] In-Context Learning for Causal Effect Estimation — https://letter-night.tistory.com/1079
- [CausalPFN] Amortized Causal Effect Estimation via In-Context Learning — https://letter-night.tistory.com/1189
- [CausalFM] Foundation Models for Causal Inference via PFNs — https://letter-night.tistory.com/1193
- [복잡한 DAG-structure로 in-context learning 하면..?](2026-01-06-complex-dag-in-context-learning.md)

## 에이전트 노트
