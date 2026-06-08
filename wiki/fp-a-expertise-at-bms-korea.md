---
title: "FP&A Expertise at BMS Korea"
tags: ["FP&A", "BMS", "finance", "PVE", "SAP", "variance-analysis", "Eliquis", "Camzyos", "Baraclude", "pharma", "GTN", "MATP"]
created: 2026-06-08T10:04:56.963Z
updated: 2026-06-08T10:04:56.963Z
sources: ["claude/conversations.json", "claude/memories.json"]
links: ["startup-projects.md", "career-background-and-profile.md"]
category: reference
confidence: high
schemaVersion: 1
---

# FP&A Expertise at BMS Korea

# FP&A Expertise at BMS Korea

## Role & Responsibilities
Finance/FP&A Manager at Bristol Myers Squibb (BMS) Korea since ~February 2026, covering:
- Cardiovascular: Eliquis (apixaban), Camzyos (mavacamten)
- Hepatitis B: Baraclude
- Cross-functional: APAC finance team (Jose, Val, Kalyan), CLO/EY project

## Core Frameworks

### PVE (Price Volume Effect) Decomposition
Decompose revenue variance into: Price effect + Volume effect + GTN (Gross-to-Net) effect
- **Eliquis key case**: Driver report showed +$0.1M favorable GTN but MATP analysis showed unfavorable (-18M KRW). B/S accrual movement (~30M KRW) had NO P&L impact. Root cause: SAP transaction-level pull needed.
- **Camzyos key insight**: Reported NTS was negative due to return drag, but ex-returns was actually favorable (+$181k vs. budget). Never conclude on reported NTS alone.
- **Baraclude PVE**: 1.0mg had severe volume shortfall (actual ~21% of P1), while 0.5mg had favorable price variance offsetting volume losses.

### SAP Operations
- Cross-rate formula: EUR/KRW = EUR→USD ÷ (KRW→USD ÷ KRW Ratio=100)
- Document types: ZDMR (Debit Memo Request), ZP (payment), K9 (linked clearing)
- Navigation: FB03 (document display), FBL1N (vendor line items), Clearing Document lookup
- AR metrics: Weighted Average Terms, Days Past Due (uses Posting Date, not Baseline Date)
- Autobank PSS setup for Korea (profit center NOT used for payment posting)

### Commentary Style Rule
**Format: cause + context** in one concise English line
- Terminology: phasing, sell-out, true-up, demand, inventory
- Abbreviations: 1L (first line), mPC (metastatic prostate cancer), QTD, YTD, ex-fac
- Never start consecutive sentences with "As"

## CLO/EY AR Reporting
Seven AR metrics defined by EY; Power BI dashboard by Val, commentary coordinated by Jose.
When AR balance is negative (customer overpayment), all three metrics = N/A.

## Key Insight
**Surface-level reporting hides the truth.** Decomposition is not optional — Camzyos appeared negative on NTS but was actually favorable ex-returns. Eliquis GTN appeared favorable in driver report but was unfavorable in underlying data. Always decompose before concluding.

## Cross-references
[[Startup-Projects]] [[Career-Background-and-Profile]]
