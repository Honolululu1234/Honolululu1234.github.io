---
title: "AI and Tech Development Skills"
tags: ["Claude-Code", "gstack", "AI", "tech", "Next.js", "Streamlit", "multi-agent", "voice-AI", "machine-learning", "KAIST", "Vercel", "Python"]
created: 2026-06-08T10:05:55.032Z
updated: 2026-06-08T10:05:55.032Z
sources: ["claude/conversations.json", "claude/memories.json"]
links: ["startup-projects.md", "fp-a-expertise-at-bms-korea.md"]
category: pattern
confidence: high
schemaVersion: 1
---

# AI and Tech Development Skills

# AI and Tech Development Skills

## Claude Code & Agentic Workflow

### Core Concepts
- **Spec-Driven Development (SDD)**: Write spec before coding. Persists across sessions (unlike Plan Mode which is temporary).
- **Plan Mode**: Read-only analysis mode. Enter via Shift+Tab (twice) or `/plan` command. Windows bug: Shift+Tab may skip Plan Mode → use `/plan`.
- **gstack**: YC-style skill pack by Garry Tan (garrytan/gstack on GitHub). 23 expert persona slash commands.
  - `/office-hours`: Reviews project direction. Output: biggest lesson, one action item, result.
  - `/plan-ceo-review`, `/plan-eng-review`, `/plan-design-review`: Review from different angles.
  - SLC framework: Simple, Lovable, Complete.

### Workflow Pattern (KAIST AI-Driven Business course)
Spec → Review (gstack) → Implement → Test → Commit (PR)

### Windows Setup Notes
- Native installer: `irm https://claude.ai/install.ps1 | iex`
- Install path: `C:\Users\User\.local\bin`
- Requires manual PATH addition
- PowerShell 7 needed for hooks: `winget install Microsoft.PowerShell`
- clawd-on-desk: Windows 11 desktop pet reacting to Claude Code session states

---

## Multi-Agent Architecture Pattern
**말하는 비서실** demonstrates the pattern:
- Orchestrator routes to specialized subagents by role
- Two-layer prompts: universal rules (Layer 1) + domain knowledge (Layer 2)
- API keys in `.env.local` (never commit); share `.env.local.example` with team

### Key Agents in PharmaOnboard
Orchestrator → [Product Knowledge | Terminology | Business Processes | Quiz | Progress Tracking]

---

## Tech Stack Knowledge

### Python/Streamlit
- Lower barrier than React: only needs Python knowledge
- Re-runs entire script on interaction (no manual state management)
- Trade-off: less flexible, not for complex/production-scale apps

### Next.js / Vercel
- Vercel: cloud platform for frontend deployment; GitHub-based auto-deploy; behind Next.js
- Similar services: Netlify, AWS Amplify, GitHub Pages
- `.env.local` for secrets; never commit

### Voice AI Stack (말하는 비서실)
- **STT**: Deepgram (Korean voice recognition)
- **LLM**: Claude Sonnet (Anthropic)
- **TTS**: OpenAI gpt-4o-mini-tts
- Common bug: emoji-based icons fail in Next.js → use lucide-react library

---

## ML Concepts (KAIST Coursework)
- **Overfitting prevention**: dropout, regularization, early stopping, data augmentation
- **RNN**: sequential data; parameter count depends on hidden size and input dimensions
- **CNN output size**: (input - kernel + 2*padding) / stride + 1
- **Model evaluation**: accuracy, precision, recall, F1, AUC-ROC

---

## GitHub & Collaboration
- Branch workflow: feature branches → PR → review → merge
- CLAUDE.md: project context file for Claude Code
- GitHub Pages: deploy static sites from `username.github.io` repo

## Cross-references
[[Startup-Projects]] [[FP&A-Expertise-at-BMS-Korea]]
