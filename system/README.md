# The AI system (phase 1: requirements and design drafts)

A multi-agent system that **finds niches, plans, creates, distributes and sells digital products**,
mostly by itself, with the **operator approving key decisions**.

> Status: phase 1. Start with **[requirements.md](requirements.md)**. Tools are chosen in
> phase 2 and the pipeline is built in phase 3.

## Agents

| # | Agent | Job | Output |
|---|---|---|---|
| 1a | **Demand Research** | What people need and search for: pain, urgency, recurring questions | Problems and pockets with evidence |
| 1b | **Bestseller Research** | What sells best now: products, formats, prices, sales signals. Extract the idea to make a better product | Proven product patterns |
| 2 | **Niche Scoring & Product Planning** | Combine demand and bestseller evidence, score opportunities (demand, proof of payment, gap, price, reach). Decide which products to make | Ranked product plan ✋ |
| 3 | **Product Creation** | Write and design the product (PDF, template, guide, Notion…) | Product draft ✋ |
| 4 | **Distribution & Marketing** | Find the communities where buyers gather, write posts and listings, follow each platform's rules | Distribution plan and posts ✋ |
| 5 | **Sales & Delivery** | Product listing, pricing, automated delivery (Whop or similar), customer support | Live product ✋ |
| 6 | **Analytics & Feedback** | Track sales, refunds and feedback. Feed what was learned back into agents 1–2 | Weekly report |

An **orchestrator** runs the pipeline, schedules agents and pauses at approval gates (✋).

## Operator approval gates ✋
- Entering a niche or starting a product
- Publishing a product (quality sign-off)
- Any public posting in communities
- Any spending (ads, tools, subscriptions)
- Price changes and refunds above a threshold

## Niche-finding mechanism and product planning (v1)
Full design: [niche-finding.md](niche-finding.md).
- **Scoring model v1 (0–100):**
  - 14 criteria, each scored 1–5 and weighted.
  - The course's five unlocks carry 45%. Demand proof, ability to pay and solution gap carry 26%.
    Reach plus a new **warm access to buyers** factor carry 17%. Verifiability, evidence base,
    effort and risk carry 12%.
  - **Hard gates:** pain, specificity, **demand proof (searched + paid)**, access to buyers,
    operator verifiability, evidence base, policy risk.
  - **Thresholds:** 75+ recommend, 65–74 cheap test, 55–64 needs evidence.
  - **Kill rules:** a 21-day launch test.
- **Pipeline:**
  - Steps: seeds → pockets → one evidence pack per niche in `research/niches/<slug>/` → scoring →
    promise and ranked plan in `products/plan/` → ✋ G1 → hand-off to `products/<slug>/`.
  - Data collection is automated only where platform terms allow it. The rest is a manual checklist.
  - Cost is about $15 a week of LLM spend and about 1–1.5 h a week of operator time.
- **Product-planning agent:**
  - Ranks the scored niches, with a first-sale rule (warm access and a short build come first).
  - Balances the portfolio, picks formats and sets prices on a ladder (free sample → $19–49 →
    $79–149 → team licence).
- **MVP:** three weekly Claude Code routines with file-based state. The operator approves in
  `system/approvals/queue.md` until a Telegram bot exists.

## Open questions
- Framework and stack (see the research report)
- Which data sources we can legally and reliably automate
- How approvals reach the operator (Telegram, email, dashboard?)
- Budget limits for LLM and API costs
