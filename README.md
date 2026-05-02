# Olugu Kalu King

**Principal & Lead Developer · ACE College International · Lagos, Nigeria**

> *"I came to software engineering at 45, not 22 — which means every system
> I have built has been immediately accountable to real students, real parents,
> and real institutional consequences. I have never had the luxury of
> building in a sandbox."*

---

## What I Build

I am a self-taught full-stack engineer and school principal in Ikorodu,
Lagos, Nigeria. My deployment environment is a live secondary school
serving 260+ students and 30+ staff — which means every system I ship
is immediately stress-tested by real institutional operations: fee
collection, student performance tracking, staff accountability, and
parental communication.

I also build algorithmic trading systems that run on a live broker
account — where unreliable code costs real money.

Both contexts produce the same discipline: build it right the first
time, because there is no safe place for it to fail.

---

## Production Systems

### 🏫 School Operations — ACE College International

| Repository | What It Does | Stack |
|---|---|---|
| [ace-sabi-api](https://github.com/ACECollegeInternational/ace-sabi-api) | School intelligence API — at-risk student detection, parent notifications, RBAC-gated staff commands | FastAPI · Python · MySQL · Telegram |
| [ace-bursar-bot](https://github.com/ACECollegeInternational/ace-bursar-bot) | WhatsApp fee automation for 300+ students — zero vendor cost | n8n · WhatsApp Business API · MySQL |
| [ace-touch-typer](https://github.com/ACECollegeInternational/ace-touch-typer) | 143-lesson gamified typing curriculum on a local Docker stack | HTML · JS · Docker · Nginx |
| [ace-essaymaster-pro](https://github.com/ACECollegeInternational/ace-essaymaster-pro) | Gemini 2.0 Flash AI writing tutor — live JSS3 classroom deployment | HTML · JS · Gemini 2.0 Flash |
| [ace-server-stack](https://github.com/ACECollegeInternational/ace-server-stack) | Full school intranet on a ₦120k laptop — JupyterHub + OnlyOffice | Docker Compose · Nginx · MikroTik |
| [ace-gamified-lessons](https://github.com/ACECollegeInternational/ace-gamified-lessons) | 7+ standalone AI-integrated gamified lesson applications | HTML · JS · Web Audio · Gemini |

### 📈 Algorithmic Trading

| Repository | What It Does | Stack |
|---|---|---|
| [fxguru-smc-ea](https://github.com/ACECollegeInternational/fxguru-smc-ea) | MQL5 Expert Advisor with four-state machine architecture — live Exness MT5 account | MQL5 · MetaTrader 5 · REST API |
| [ai-signal-bot](https://github.com/ACECollegeInternational/ai-signal-bot) | Extended fork — SMC confluence scoring engine, multi-provider LLM
fallback chain, and fundamental analyst filter built on an open-source
foundation | FastAPI · Python · Groq · Anthropic · Gemini |
| [ngx-research-bot](https://github.com/ACECollegeInternational/ngx-research-bot) | Six-role multi-agent LLM equity research pipeline for the Nigerian Exchange | n8n · LLM APIs · Google Sheets |

## Acknowledgements

The project ai-signal-bot began as a fork of work by [Citycod],
whose original codebase provided the initial signal request structure.
The system has since been substantially extended beyond that foundation —
including the SMC confluence scoring engine, multi-provider LLM fallback
chain, Pydantic response validation layer, fundamental analyst filter,
structured JSON output schema enforcement, and Render deployment
configuration. All extensions are original work.

The original repository: [(https://github.com/Citycod/trading-bot)]

---

## Technical Stack
Languages       Python 3.11 · MQL5 · JavaScript (ES6+) · HTML5 · CSS3
Frameworks      FastAPI · n8n · Node.js
Databases       MySQL 8.0 · Three-schema federation
Infrastructure  Docker Compose · Ubuntu 24.04 · Caddy · Nginx · MikroTik
AI / LLM        Gemini 2.0 Flash · Anthropic Claude · Groq API
Messaging       WhatsApp Business Cloud API · Telegram Bot API · OpenClaw
Trading         MetaTrader 5 · Exness Broker · MQL5 state machines
Hosting         Contabo VPS · Render · Local school server (HP Envy x360)

---

## The Architecture Decisions I Am Known For

**Federation over migration**
The Sabi API reads across three live MySQL schemas at query time
rather than migrating 13 years of institutional data into a unified
store. The integration layer is the engineering problem — not the data.

**Maintainability over cleverness**
n8n over custom Flask handlers. Admin panels that let a bursar
change a message template without touching code. Systems designed
to survive beyond direct developer involvement — because in a
single-person IT department, that is not a nice-to-have.

**Single-file deployment for constrained environments**
Every classroom tool ships as one HTML file with zero external
CDN dependencies. Lagos classrooms have unreliable internet.
The tools work anyway.

**State machines for stateful problems**
The FxGuru EA runs inside MT5's tick-driven event loop — which
calls OnTick() hundreds of times per minute. A four-state machine
(BOOT → POLLING → DATA_PUSH → ERROR_RECOVERY) ensures each action
executes exactly once per cycle, with predictable fault isolation
that never touches open positions during recovery.

---

## By The Numbers
9      Production systems built and maintained
260+   Students served by the school operations stack
143    Lessons in the ACE Touch Typer curriculum
3      MySQL schemas federated by the Sabi API without migration
4      LLM providers integrated across the trading and EdTech stacks
0      External IT vendors. Everything built in-house.
₦0     Recurring software licensing cost for the school intranet stack

---

## Community

**studypalNG** — YouTube channel for Nigerian students and educators.
Expanding in 2026 to document school operations automation, AI
classroom tools, and EdTech infrastructure builds — making the
technical journey visible to Nigerian school owners and developers
who face the same problems.

▶ [youtube.com/@studypalNG](https://youtube.com/@studypalNG)

---

## Background

Self-taught trajectory beginning in 2019 — from PHP scripting to
FastAPI microservices, MQL5 state machines, multi-provider LLM
pipelines, and Docker Compose infrastructure stacks.

No CS degree. Every skill acquired under production pressure,
with real institutional or financial consequences for getting
it wrong.

Active member and speaker, Full Gospel Business Men's Fellowship
International (FGBMFI) — a global network with chapters across
Nigeria and the United Kingdom.

---

## Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-kalu--olugu-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/kalu-olugu)
[![YouTube](https://img.shields.io/badge/YouTube-studypalNG-FF0000?style=flat&logo=youtube&logoColor=white)](https://youtube.com/@studypalNG)
[![Organisation](https://img.shields.io/badge/GitHub_Org-ACE_College_International-181717?style=flat&logo=github&logoColor=white)](https://github.com/ACECollegeInternational)

---

*All production credentials, student data, and broker configurations*
*are excluded from public releases.*
*See individual repository* `SECURITY.md` *files for details.*
