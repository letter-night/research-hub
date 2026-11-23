---
type: paper
title: "Learning Stochastic Dynamics from Snapshots through Regularized Unbalanced Optimal Transport"
authors: ""
year: 2025
venue: "ICLR 2025"
url: ""
topics: [generative-models]
tags: [single-cell, unbalanced-ot, schrodinger-bridge]
status: read
date: 2026-08-26
builds_on: []
my_rating:
source_post: https://letter-night.tistory.com/1463
migration: summary
migrated: 2026-11-23
---

# Learning Stochastic Dynamics from Snapshots through Regularized Unbalanced Optimal Transport

**기존 글**
- [Learning Stochastic Dynamics from Snap-shots through Regularized Unbalanced OT](https://letter-night.tistory.com/1463) (2026-08-26)
- [Learning Stochastic Dynamics from Snapshots through Regularized Unbalanced OT](https://letter-night.tistory.com/1469) (2026-08-29)

## 한 줄 요약

## 핵심 내용

## 나의 리뷰
*(2026-08-26 글 "[thought] Deep RUOT를 보고 든 생각"에서 옮김)*
- 세상에 공짜는 없다. cell의 birth/death를 반영한 realistic한 stochastic dynamics 모델링은 최적화할 parameter 수를 늘리고, 안정적인 학습을 위해 hyperparameter 조율을 요구한다.
- SB는 SDE/ODE solver 시뮬레이션이 필요해서 고차원 cell state에서는 학습이 특히 까다롭다.
- 학습 효율을 높이려면 cell의 **latent embedding space에서 ODE를 시뮬레이션**하면 어떨까? (저자들도 future direction으로 제시)
- multi-modality를 반영하면 어떨까?

## 열린 질문 / 한계

## 연결

## 에이전트 노트
