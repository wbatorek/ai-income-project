# The AI system (design, draft v0)

A multi-agent system that **finds niches, plans, creates, distributes and sells digital products**,
mostly by itself, with the **operator approving key decisions**.

> Status: draft. To be refined with
> [research/self-running-ai-system.md](../research/self-running-ai-system.md) (in progress) and the
> Episode 2 analysis of product types and how buyers decide (course/sessions/02-develop.md).

## Agents

| # | Agent | Job | Output |
|---|---|---|---|
| 1 | **Market & Trend Research** | Scan markets, communities and bestseller lists. Spot rising demand and underserved problems | Niche candidates with evidence |
| 2 | **Niche Scoring & Product Planning** | Score niches (demand, competition, buyer intent, price, distribution access, fit with our skills). Decide which products to make | Ranked product plan ✋ |
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

## Niche-finding mechanism (to design after Episode 2)
Inputs: course knowledge on product types and buyer decisions, plus our market research.
Output: a repeatable scoring model and a pipeline that produces a ranked list of product
opportunities each week.

## Open questions
- Framework and stack (see the research report)
- Which data sources we can legally and reliably automate
- How approvals reach the operator (Telegram, email, dashboard?)
- Budget limits for LLM and API costs
