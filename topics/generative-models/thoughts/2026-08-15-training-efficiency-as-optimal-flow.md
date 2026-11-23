---
type: thought
title: "generative model의 training efficiency: 학습을 optimal flow로 볼 수 있을까 (thought 1, 2)"
topics: [generative-models]
tags: [training-dynamics, optimal-transport, flow-matching, fokker-planck]
date: 2026-08-15
source_post: https://letter-night.tistory.com/1433
migration: summary
migrated: 2026-11-23
---

# generative model의 training efficiency: 학습을 optimal flow로 볼 수 있을까 (thought 1, 2)

> 기존 블로그 글에서 옮긴 요약입니다. 원문 표현을 최대한 살렸지만 전문은 아닙니다.
- [[thought] generative model의 training efficiency에 대해서](https://letter-night.tistory.com/1433) (2026-08-04)
- [[thought 2] generative model의 training efficiency에 대해서](https://letter-night.tistory.com/1444) (2026-08-15)

## 나의 생각
**thought 1 (2026-08-04)**
- 연속방정식과 Fokker-Planck 방정식을 쓰면 입자의 궤적뿐 아니라 확률밀도의 변화도 알 수 있다.
- SDE formulation을 같은 probability path를 만드는 ODE로 바꾸면 학습과 추론을 효율적이고 안정적으로 만들 수 있다.
- Flow Matching으로 확장하면 임의 분포 사이의 transport를 다룰 수 있다.
- 생성 모델링은 $p_{\text{model}}$과 $p_{\text{data}}$ 사이의 discrepancy를 줄이는 과정이다. 학습은 모델 분포의 **확률 질량을 어떻게 옮길지**의 문제다.

**thought 2 (2026-08-15)**
- generative modeling = model distribution을 data distribution으로 옮기는 문제. 핵심은 probability density mass를 어떻게 옮길 것인가.
- parameter update의 누적을 distribution의 변화 과정, 즉 **flow**로 보면: **어떤 training algorithm이 optimal transport(optimal flow)가 되는가?**
- 제안: optimal transport를 가정하고, 모델 $p_\theta$의 parameter update에 따른 분포 변화가 이 optimal flow를 따르도록 만들 수 있을까?
- 이거 말이 되는 건가요?

## 질문
- parameter space의 gradient flow와 distribution space의 Wasserstein gradient flow는 어떤 관계인가? (→ Wasserstein gradient flow 글과 연결)

## 연결된 자료

- Derivation of continuity eqn & Fokker-Planck eqn — https://letter-night.tistory.com/1428
- Understanding Girsanov's theorem intuitively — https://letter-night.tistory.com/1442
- [on-going] The Principles of Diffusion Models — https://letter-night.tistory.com/1431

## 에이전트 노트
