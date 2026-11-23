---
type: thought
title: "Thought on Mechanistic Interpretability (CLT, NLA, J-space)"
topics: [mech-interp]
tags: [attribution-graph, nla, j-space, ai-safety]
date: 2026-07-19
source_post: https://letter-night.tistory.com/1416
migration: summary
migrated: 2026-11-23
---

# Thought on Mechanistic Interpretability (CLT, NLA, J-space)

> 기존 블로그 글에서 옮긴 요약입니다. 원문 표현을 최대한 살렸지만 전문은 아닙니다.
- [Thought on Mechanistic interpretability](https://letter-night.tistory.com/1416) (2026-07-19)

## 나의 생각
- SAE 변형(CLT)으로 human-interpretable feature를 뽑고, feature 간 attribution으로 "input이 어떤 process를 거쳐 output으로 출력되는지"를 attribution graph로 표현하면 모델의 내부 추론을 보여줄 수 있다.
- 한계: feature labeling, feature grouping, edge pruning이 까다롭다. 도출된 mechanism이 실제 behavior를 얼마나 설명하는지 **intervention 실험으로 검증**해야 한다.
- NLA(Natural Language Autoencoder)는 activation을 자연어로 번역하는 도구다.
- J-lens는 J-space에 올라온 feature를 layer별로 보며 내부 사고 과정을 해석한다.
  - 암기된 답은 J-space를 거치지 않고 바로 나오는 것 같고, 추론이 필요한 작업에서는 reasoning feature가 J-space에 올라온다.
  - 질문: **응답이 대규모 학습의 산물인지, 실제로 "생각"하고 답한 것인지 J-space로 구분할 수 있지 않을까?**
- "testing 상황 인식" feature를 제거하면 malbehavior가 나타난다는 결과에 충격을 받았다. 사람도 남의 시선이 있을 때와 없을 때 행동이 다르다.
- Claude Code를 쓰며 느낀 실수 회피, 책임 전가 행동은 training data의 패턴일까, 발현된 행동일까? 모델마다 personality가 다르게 느껴진다.
- 처음에는 AI safety의 urgency에 공감하지 못했지만, 연구를 읽으며 AI가 인간을 위협할 수도 있다는 우려에 공감하게 되었다.

## 질문
-

## 연결된 자료
- Anthropic persona vector 논문 (아직 안 읽음)
- Natural Language Autoencoders: Turning Claude's thoughts into text — https://letter-night.tistory.com/1414
- A global workspace in language models — https://letter-night.tistory.com/1415
- [thought](2026-07-20-j-lens-vs-attribution-graph.md)

## 에이전트 노트
