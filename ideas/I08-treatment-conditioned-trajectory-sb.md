---
type: idea
id: I08
title: "Schrödinger Bridge × Causality: treatment에 따른 trajectory 모델링"
topics: [generative-models, causality]
status: seed
proposed_by: me
origin: [1515, 1465, 1470, 1463]
date: 2026-08-26
updated: 2026-11-23
---

# I08. Schrödinger Bridge × Causality: treatment에 따른 trajectory 모델링

**출발점이 된 기록**
- [그냥 문득 든 생각들](../topics/agentic-ai/thoughts/2026-11-14-random-thoughts-ontology-and-work-knowledge.md)
- [[thought] Deep RUOT를 보고 든 생각](../topics/generative-models/papers/2025-ruot-stochastic-dynamics-snapshots.md)
- [(1/5) Reconstructing Growth and Dynamic Trajectories from Single-Cell Transcriptomics Data](../topics/generative-models/papers/2024-reconstructing-growth-dynamic-trajectories-scrna.md)
- [Learning Stochastic Dynamics from Snap-shots through Regularized Unbalanced OT](../topics/generative-models/papers/2025-ruot-stochastic-dynamics-snapshots.md)

## 질문
SB / unbalanced OT로 cell trajectory를 재구성하는 방법에 **인과적 개입(treatment)** 을 결합하면, 처치에 따른 trajectory의 반사실적 변화를 모델링할 수 있는가?

## 왜 중요한가
- 생성모델(dynamics)과 시변 처치효과(I04)를 잇는 다리. 의료 trajectory 문제에도 같은 틀을 쓸 수 있다.

## 고려할 점
- 고차원 state에서 SDE 시뮬레이션 비용 → latent space에서 시뮬레이션 (RUOT 메모)
- multimodality 반영

## 다음 한 걸음
- perturbation(처치) 조건부 single-cell trajectory 연구 현황 조사 (Research 에이전트)

## 에이전트 노트
- **[2026-11-23 · Management]** 기존 블로그 기록에서 추출해 아이디어로 정리했습니다. 문장은 연구자의 글에서 가져왔고, "접근 방법 후보"와 "다음 한 걸음"의 일부는 에이전트가 정리한 것입니다.
