---
type: thought
title: "DM/FM/SB를 공부하며: controllability는 결국 score 문제"
topics: [generative-models]
tags: [guidance, steering, sampling, solver]
date: 2026-09-12
source_post: https://letter-night.tistory.com/1484
migration: summary
migrated: 2026-11-23
---

# DM/FM/SB를 공부하며: controllability는 결국 score 문제

> 기존 블로그 글에서 옮긴 요약입니다. 원문 표현을 최대한 살렸지만 전문은 아닙니다.
- [[잡담] DM/FM/SB를 공부하며](https://letter-night.tistory.com/1484) (2026-09-12)

## 나의 생각
- 후반부 controllability(steering)의 핵심은 **score 문제**다. log potential의 기울기로 trajectory를 조종하는 것이 DM/FM/SB 전반의 철학이다: $\nabla_x \log \phi(x)$
- 목표 에너지 함수는 density에 constraint의 지수를 곱하는 방식으로 만든다: $p_{\text{target}}(x) \propto \rho(x)\, e^{-c(x)}$
- trajectory 계산은 코바늘 뜨기 같다. 수치 적분 방식에 따라 accuracy와 efficiency 사이에 trade-off가 생긴다.
- fast sampling은 고급 solver의 인스턴스화로 볼 수 있다. 세부 계산은 인내가 필요하다.
- Distillation은 이해했지만 DPM-solver 이후는 아직이다. 10월 수업 내용을 복습할 계획.

## 질문
-

## 연결된 자료

- DM Cheat Sheet — https://letter-night.tistory.com/1498
- [흥미로운 공통점 찾음! (Distribution Matching)](2026-08-17-sb-and-dpg-same-form.md)

## 에이전트 노트
- **[2026-11-23 · Management]** 원문 앞부분의 개인적인 이야기(좋은 인연, 동료에 대한 감사)는 이전하지 않았습니다.
