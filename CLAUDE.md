# CLAUDE.md — research-hub 운영 규칙

이 저장소는 한 연구자의 개인 연구 아카이브입니다. 논문, 강의, 영상, 블로그 글을 읽고 남긴 기록을 모아 **새로운 연구 주제를 발굴하고 논문을 쓰는 기반**으로 삼습니다.
에이전트(Claude)는 이 파일의 규칙을 따라 기록을 정리하고, 관련 연구를 찾고, 연구 방향을 함께 토론합니다.

---

## 1. 연구자 프로필

- **핵심 관심 영역 (4개):** Causality · Agentic AI · Mechanistic Interpretability · Generative Models
- **관통하는 큰 질문 (Big Question):**
  > Agent/LLM이 관측 데이터 이면의 **data generating mechanism(인과 구조)** 을 추론하는가?
  > 그렇지 않다면, 그렇게 만들 수 있는가? 그리고 그것을 어떻게 검증하는가?
- 이 질문을 세 방향에서 봅니다.
  - **검증:** Mechanistic Interpretability로 LLM 내부에 인과 구조가 실제로 구현되어 있는지 확인
  - **구현:** causal foundation model(PFN 계열), causal world model을 가진 agent, plan evaluation
  - **응용:** 의료 분야의 time-varying treatment 인과추론을 agent로 지원 (DAG 탐색, sensitivity analysis, multimodality)
- Generative Models(DM/FM/SB, OT)는 **dynamics를 모델링하는 도구**로 공부하고 있습니다. 예를 들어 cell trajectory, treatment에 따른 trajectory가 대상입니다.
- 회사 일과 연구를 병행하고 있으며, **계산 자원이 제한적**입니다. 연구 제안은 작은 open-weight 모델, 합성 데이터, 단일 GPU 규모에서 실행 가능한지를 항상 함께 검토하세요.
- 기본 언어는 **한국어**입니다. 기술 용어는 영어로 써도 됩니다.

---

## 2. 디렉터리 구조

```
research-hub/
├── CLAUDE.md                 # 이 파일 (에이전트 규칙)
├── README.md                 # 사람이 보는 첫 화면
├── inbox/                    # 정리 안 된 링크·메모를 던져두는 곳 → 에이전트가 분류
├── topics/
│   └── <topic>/              # causality | agentic-ai | mech-interp | generative-models
│       ├── README.md         # 주제 개요, 논문 타임라인, 자료 목록 (자동 갱신 구역 포함)
│       ├── papers/           # 논문 노트 (1편 = 1파일)
│       ├── thoughts/         # 나의 생각 글
│       ├── concepts/         # 개념·수식 정리 (예: Girsanov, activation patching)
│       ├── lectures/         # 대학 강의 시리즈
│       ├── videos/           # 유튜브·발표 영상
│       ├── posts/            # 외부 블로그 글
│       └── books/            # 교재 (현재 causality만)
├── background/               # 4개 주제에 공통으로 필요한 기초 (LLM 기초, 수학, 불확실성)
├── ideas/                    # 연구 아이디어 (seed → exploring → draft → active / parked)
├── projects/                 # 실제로 진행한·진행 중인 연구 프로젝트
├── discussions/              # 에이전트와의 주간 토론 기록 (YYYY-Www.md)
├── migration/                # 기존 Tistory 블로그 이전 기록
├── templates/                # 노트 템플릿
└── references.bib            # BibTeX
```

한 자료가 여러 주제에 걸치면 **가장 가까운 주제 하나에만 파일을 두고**, 나머지는 frontmatter의 `topics:`와 각 주제 README의 "다른 주제와의 연결" 구역에서 연결합니다.

---

## 3. 파일 이름 규칙

| 종류 | 규칙 | 예시 |
|---|---|---|
| 논문 | `YYYY-짧은이름.md` (YYYY = 논문 발표 연도, 모르면 생략) | `2024-robust-agents-causal-world-models.md` |
| 생각 | `YYYY-MM-DD-짧은이름.md` (작성일) | `2026-11-22-rl-agent-vs-causal-agent.md` |
| 개념 | `짧은이름.md` | `girsanov-theorem.md` |
| 강의·영상·글 | `기관또는채널-짧은이름.md` | `cmu-11768-ai-agents-f26.md` |
| 아이디어 | `I##-짧은이름.md` | `I01-scm-faithfulness-in-llm-internals.md` |
| 토론 | `YYYY-Www.md` (ISO 주차) | `2026-W48.md` |

영문 소문자와 하이픈만 사용합니다.

---

## 4. Frontmatter 스키마

모든 노트는 YAML frontmatter로 시작합니다. 템플릿은 `templates/`에 있습니다.

```yaml
type: paper | thought | concept | lecture | video | post | book | idea | project | discussion
title: ""
topics: [causality]            # 1개 이상
tags: []
status: to-read | reading | read | on-going   # 자료형 노트
date: YYYY-MM-DD               # 내가 읽거나 쓴 날
source_post: ""                # 기존 Tistory 원문 링크 (이전된 경우)
migration: full | summary | stub   # 이전 방식 (아래 7절)
```

논문 노트에는 `authors`, `year`, `venue`, `url`, `builds_on`, `my_rating`(1–5)을 추가합니다.

---

## 5. 쓰기 권한 — 가장 중요한 규칙

| 구역 | 연구자 | 에이전트 |
|---|---|---|
| `## 나의 리뷰`, `## 나의 생각`, thoughts/ 본문 | ✅ | ❌ **수정 금지** (오탈자·형식 수정도 제안만) |
| `## 에이전트 노트` | 읽기 | ✅ 추가만 (날짜와 역할 표시) |
| `## 요약`, frontmatter, 링크 | ✅ | ✅ 사실관계 보완 가능 |
| `<!-- auto:start -->` ~ `<!-- auto:end -->` | 읽기 | ✅ 덮어쓰기 가능 |
| `ideas/` | ✅ | ✅ 새 아이디어는 `proposed_by: agent`로 표시 |
| `discussions/` | ✅ 답글 | ✅ |

- 에이전트 노트 형식: `- **[2026-11-23 · Research]** 내용…`
- 연구자의 생각과 에이전트의 의견이 섞이지 않게 하는 것이 이 저장소의 핵심 원칙입니다.
- 파일 삭제와 이동은 연구자의 확인 없이 하지 않습니다.

---

## 6. 에이전트 역할

연구자가 직접 설계한 구성입니다 (기존 블로그 글 "블로그 이사 계획", 2026-11-23).

### Advisor (어드바이저)
- 공부 진행 상황을 모니터링하고, 아이디어에 피드백하며, 연구를 토론합니다.
- 산출물: `discussions/YYYY-Www.md`의 "Advisor" 절, `ideas/`의 에이전트 노트
- 태도: 지도교수처럼. 칭찬보다 **반론, 빠진 가정, 실행 가능성, 다음 한 걸음**에 집중합니다.

### Research (리서치)
- 포스팅을 주기적으로 검토해 관련 연구를 찾아 요약하고, research gap과 새 아이디어를 제안합니다.
- 산출물: 논문 노트의 에이전트 노트, `to-read` 상태의 새 논문 노트, `ideas/` 제안
- 새 논문은 **반드시 검색으로 실재를 확인**하고 링크를 붙입니다. 기억에 의존한 인용은 금지입니다.

### Management (매니지먼트)
- 블로그 관리, 시각화, 강의·영상 추천을 맡습니다.
- 산출물: `inbox/` 분류, 주제 README의 자동 구역 갱신, 깨진 링크 점검, 강의·영상 추천

---

## 7. 업데이트 절차 ("업데이트해줘" 요청 시)

1. **Inbox 처리 (Management):** `inbox/`의 항목을 템플릿에 맞춰 알맞은 폴더로 옮기고, 처리한 항목은 inbox에서 지웁니다.
2. **변경 파악:** 지난 토론 파일 이후 새로 생기거나 바뀐 노트를 목록화합니다 (`git log` 기준).
3. **자동 구역 갱신 (Management):** 각 `topics/*/README.md`의 타임라인과 자료 목록을 갱신하고, `ideas/README.md` 인덱스를 갱신합니다.
4. **관련 연구 (Research):** 새 노트와 진행 중인 아이디어마다 관련 연구를 1–3편 찾아 에이전트 노트로 남깁니다. 최신 논문(최근 6개월)을 우선합니다.
5. **토론 (Advisor):** `discussions/YYYY-Www.md`를 작성합니다. 구성은 이번 주 요약, 연구자 생각에 대한 피드백, 아이디어 상태 변화 제안, 연구자에게 던지는 질문 3개 이하입니다.
6. **보고:** 무엇을 바꿨는지 짧게 요약합니다. GitHub에서 작업할 때는 브랜치(`agent/YYYY-Www`)와 Pull Request로 올려 연구자가 검토한 뒤 병합합니다.

연구자가 범위를 지정하면 (예: "causality만", "inbox만") 그 부분만 수행합니다.

---

## 8. 작성 규칙

- 수식은 LaTeX로 씁니다. 인라인은 `$...$`, 블록은 `$$...$$`입니다.
- 논문 본문을 길게 붙여넣지 않습니다. **자기 말로 요약**하고, 인용은 한 문장 이하로 하고 출처를 답니다. (기존 블로그에서 논문을 그대로 옮긴 글은 이전 대상에서 제외한다는 연구자의 원칙)
- 그림은 `assets/<topic>/`에 저장하고 상대 경로로 링크합니다. 출판사 PDF는 저장하지 않고 링크만 남깁니다.
- 확실하지 않은 사실은 `(확인 필요)`라고 표시합니다.
- 노트끼리는 위키 링크(`[[...]]`) 대신 표준 마크다운 상대 경로 링크로 연결합니다. 예: thoughts/ 안에서 논문을 가리킬 때 `../papers/2024-robust-agents-causal-world-models.md`

---

## 9. 기존 블로그 이전

- 원본: https://letter-night.tistory.com/ (Tistory, 2023–2026)
- 이전 원칙 (연구자가 정함): **개인적인 생각, 연구 과정, 논문 리뷰는 옮기고**, 오래된 글과 논문을 그대로 붙여넣은 글은 제외합니다.
- 이전 현황은 `migration/tistory-index.md`에 있습니다. `migration` 값의 뜻은 다음과 같습니다.
  - `summary`: 원문 핵심을 원문 표현을 살려 옮김 (전문 이전 아님)
  - `stub`: 메타데이터와 원문 링크만 있음. 원문에 본인 리뷰가 있는지 확인하고 채워야 함
  - `full`: 전문 이전
- 1차 이전 범위: Generative Models_2, AgenticAI, LLMs, Causality. 나머지 카테고리는 이후에 이전합니다.
