---
title: "Startup Projects — MySkinMap, Cinderella, PharmaOnboard, 말하는 비서실"
tags: ["startup", "MySkinMap", "Cinderella", "PharmaOnboard", "skincare", "GIS", "AI", "voice-agent", "LINE", "K-beauty", "multi-agent"]
created: 2026-06-08T10:05:18.458Z
updated: 2026-06-08T10:05:18.458Z
sources: ["claude/conversations.json", "claude/memories.json"]
links: ["fp-a-expertise-at-bms-korea.md", "ai-and-tech-development-skills.md", "career-background-and-profile.md"]
category: architecture
confidence: high
schemaVersion: 1
---

# Startup Projects — MySkinMap, Cinderella, PharmaOnboard, 말하는 비서실

# Startup Projects

## MySkinMap (Top Competition Candidate)
**Concept**: GIS-based AI platform recommending climate-adaptive skincare using location + environmental data.

### Core Product
- **Skin Stress Index (SSI)**: Quantifies environmental impact on skin by region
- Primary factors: UV, PM2.5, temperature, humidity
- Research-first approach: literature review (PubMed, AAD, JID, WHO) before building SSI weights
- Patent strategy in progress; team: 노현영, 김대성, 이규민

### Value Proposition
- Top gain: emotional outcome (피부 트러블 해소 및 자신감 회복) > functional time-saving
- Trust crisis evidence: MFDS data shows 64.3% of influencers violated advertising regulations; only 4.7% of SNS-exposed consumers purchase directly through that channel
- Positioning: against ad-driven content overload, offer evidence-based personalized curation

### Architecture Vision
- GIS environmental data (EPA AirNow, NWS API, OpenWeather) + skin profile + AI clustering
- XAI (Explainable AI) for transparent recommendations
- B2B SaaS target: clinics, dermatologists, cosmetic brands

### User Research Approach
JTBD methodology: pain discovery first, solution fit testing last (avoid confirmation bias)

---

## Cinderella Project
**Concept**: LINE-based K-beauty medical tourism platform for Thai consumers seeking non-invasive procedures in Korea.

### Core Differentiators
1. LINE as primary channel (dominant in Thailand)
2. Non-invasive procedures only (compatible with short tourist stays)
3. AI cosine similarity for personalized clinic + treatment matching
4. Transparent pricing (prevents price gouging of foreign visitors)
5. Thai-language customer support

**One-line pitch**: "태국인을 위한 LINE 기반 K-뷰티 시술 AI 추천·예약 플랫폼"

---

## PharmaOnboard
**Concept**: AI-powered onboarding service for non-science background hires at global pharma companies.

### Motivation
Personal experience as a humanities-background hire at BMS struggling with product knowledge, medical terminology (CAR-T, GTN, COGS), and pharma business processes.

### Architecture
- Multi-agent: orchestrator + 5 specialized subagents (product knowledge, terminology, business processes, quiz/assessment, progress tracking)
- Phase 1 MVP: Python/Streamlit, 27 products across 5 companies, 4 working pages
- Tech stack roadmap: Next.js + Vercel + Supabase + Claude API
- Phase 4 target: B2B SaaS

---

## 말하는 비서실 (Talking Secretary's Office)
**Concept**: Voice-based multi-agent AI advisory service (real estate consulting scenario).

### Stack
- Deepgram STT (Korean speech recognition) + Claude Sonnet (LLM) + OpenAI gpt-4o-mini-tts
- Next.js application
- Three specialized agents: CFO, CSO, mentor/advisor

### Two-Layer Prompt Architecture
- Layer 1: Universal conversational rules (colloquial Korean, 2-3 sentence responses, one question at a time, natural filler words)
- Layer 2: Domain knowledge (startup funding programs: 예비창업패키지, 청년창업사관학교, 초기창업패키지, TIPS, 창업도약패키지)

### Key Insight from /office-hours
Core user pain point = **emotional isolation** in decision-making, not calculation accuracy. Solution: add "emotional anchor" rule to CFO agent prompt.

## Cross-references
[[FP&A-Expertise-at-BMS-Korea]] [[AI-and-Tech-Development-Skills]] [[Career-Background-and-Profile]]
