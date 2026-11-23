---
type: thought
title: "흥미로운 공통점: SB와 DPG는 같은 형태 (Distribution Matching)"
topics: [generative-models]
tags: [schrodinger-bridge, dpg, max-entropy, controlled-generation]
date: 2026-08-17
source_post: https://letter-night.tistory.com/1449
migration: summary
migrated: 2026-11-23
---

# 흥미로운 공통점: SB와 DPG는 같은 형태 (Distribution Matching)

> 기존 블로그 글에서 옮긴 요약입니다. 원문 표현을 최대한 살렸지만 전문은 아닙니다.
- [흥미로운 공통점 찾음! (Distribution Matching)](https://letter-night.tistory.com/1449) (2026-08-17)

## 나의 생각
- SB는 endpoint marginal constraint를 만족하면서 reference path와의 discrepancy를 최소화하는 문제이고, entropy-regularized OT와 equivalent하다. **reference path가 일종의 cost function 역할**을 한다.
- 이 형태가 DPG(Distributional Policy Gradient)와 **동일한 form**이다.

$$
\min_{p \in \mathcal{C}} \; D\!\left(p \,\|\, p_{\text{ref}}\right)
$$

- DPG: reference = pretrained LM. constraint를 만족하는 distribution family 안에서 reference와의 거리를 최소화하는 target distribution을 구한다 → **Maximum Entropy Principle의 일반화**.
- SB: reference = Brownian motion. endpoint marginal constraint 아래 KL을 최소화한다.

$$
\min_{\pi:\,\pi_0=\mu_0,\;\pi_1=\mu_1} \mathrm{KL}\!\left(\pi \,\|\, \mathbb{W}\right)
$$

- Stochastic Optimal Control 형식으로 풀면 value function이 나오는데, 그 전개가 대단히 비슷하다. 목표 constraint가 exponential family 형태로 주어지는 점도 같다.

## 질문
-

## 연결된 자료

- [KL-Adaptive DPG] Distributional Approach to Controlled Text Generation — https://letter-night.tistory.com/1328
- [CDPG] Controlling Conditional Language Models — https://letter-night.tistory.com/1330
- [SB framework 안에서 DM와 FM의 탄생 비화를 깨닫고 있다](2026-08-18-birth-of-dm-and-fm-within-sb.md)

## 에이전트 노트
