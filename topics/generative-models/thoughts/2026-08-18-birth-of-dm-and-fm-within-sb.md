---
type: thought
title: "SB framework 안에서 DM와 FM의 탄생 비화"
topics: [generative-models]
tags: [schrodinger-bridge, optimal-transport, diffusion, flow-matching]
date: 2026-08-18
source_post: https://letter-night.tistory.com/1451
migration: summary
migrated: 2026-11-23
---

# SB framework 안에서 DM와 FM의 탄생 비화

> 기존 블로그 글에서 옮긴 요약입니다. 원문 표현을 최대한 살렸지만 전문은 아닙니다.
- [SB framework 안에서 DM와 FM의 탄생 비화를 깨닫고 있다](https://letter-night.tistory.com/1451) (2026-08-18)

## 나의 생각
- Schrödinger Bridge의 해는 **forward/backward potential로 아름답게 떨어진다.**
- 그런데 비선형 PDE를 직접 풀기는 까다롭다. 그래서 한 potential을 상수로 두고 **half-bridge problem**으로 푸는 타협을 한다. 이 경우 reverse score만 추정하면 되는데, 이것이 **DM**이다.
- EOT와 OT는 모두 intractable하다. 양 끝단에서 독립적으로 샘플링한 coupling을 선형 보간하는 conditional flow는 OT 운동에너지의 **최소 상한**을 준다. 그래서 **FM**도 OT의 실용적 대안이 된다.
- 정확한 log likelihood 대신 variational lower bound를 최대화하는 것과 같은 **꿩 대신 닭**식 타협이다.
- 결론: DM과 FM 모두 OT/EOT를 풀고 싶었지만, 현실적으로 가능한 타협점을 찾은 것이다.

## 질문
-

## 연결된 자료

- Schrodinger Bridge solution as two space-time potentials — https://letter-night.tistory.com/1445
- [on-going] Foundations of SBs for Generative Modeling — https://letter-night.tistory.com/1447
- [흥미로운 공통점 찾음! (Distribution Matching)](2026-08-17-sb-and-dpg-same-form.md)

## 에이전트 노트
