# System requirements (phase 1, living document)

What the AI digital-product system must do. Tools are **not** chosen here; that is phase 2.
Every requirement cites its source: **[C]** course knowledge, **[O]** operator knowledge,
**[R]** our research, **[I]** ideas backlog.

## Goal
Make a lot of money selling digital products, with a system that researches, creates and sells
them mostly on its own, while the operator approves key decisions. [O]

## Functional requirements

### Research: two layers [O] [I #1]
- **R1 Demand research.** Find what people need and look for: problems, pain, urgency, search
  demand, recurring questions, complaints. Output "profitable pockets" with evidence. [C] [O]
- **R2 Bestseller research.** Find what currently sells best: products, platforms, formats, prices,
  sales and review signals, trends over time. [O]
- **R3 Pattern extraction.** From bestsellers, extract the *idea* (niche × format × price ×
  positioning) and propose a new, better or more specific product. Never copy content, branding or
  design. [O]
- **R4 Combine layers.** Rank opportunities that have both demand and proof of payment, plus a gap
  we can fill. [O] [C]
- **R5 Market choice.** Prefer markets where buyers *don't* solve the problem with AI themselves.
  Don't default to the operator's own professions. [O]

### Selection and planning
- **R6 Scoring.** Score opportunities with an explicit, adjustable model (first draft:
  [niche-finding.md](niche-finding.md); the course's five unlocks: pain, worsening pain,
  transformation, specificity, speed). [C]
- **R7 Product promise.** Every candidate gets "I help [who] with [worsening problem] get
  [result] in [time]". [C]
- **R8 Portfolio and pricing.** Plan a portfolio and price ladder. Expect early products to earn
  $0 and iterate. [C]

### Creation
- **R9 Synthesis.** Build products by synthesising many credible sources (course: 150+) into one
  step-by-step method, with references. [C]
- **R10 Formats.** Support ebook/PDF first, then templates, planners and other formats. [C]
- **R11 Quality.** Products must be good enough to avoid refunds and platform bans for low-quality
  AI content. [R]

### Distribution and sales (to be completed after Episode 3)
- **R12 Distribution.** Reach buyers where they gather. Automate only where platform rules allow;
  otherwise draft for the operator to post. [C] [R]
- **R13 Delivery.** Automated sales and delivery through a merchant-of-record platform (handles
  sales tax and VAT). [R] [tax/]
- **R14 Feedback.** Track sales, refunds and reviews, and feed results back into research and
  scoring. [R]

### Operator control
- **R15 Approval gates.** The operator approves: entering a niche, publishing, public posting, any
  spending, prices. Nothing happens without a decision. [O] [R]
- **R16 Transparency.** Every recommendation shows its evidence and sources.

## Non-functional requirements
- **N1 Mostly autonomous**, with a low weekly time cost for the operator. [O]
- **N2 Cost-aware.** Use the existing Claude Ultra subscription where it fits; add paid tools only
  when they're clearly better for a job. Don't buy the course's ~$2,000 offer. [O]
- **N3 Legal.** Respect platform terms of service, copyright and tax rules. [R]
- **N4 Best tool per job.** Claude isn't assumed to be best at everything (e.g. market analysis
  might be better with Perplexity or data tools). Decided in phase 2. [O]

## Open questions for phase 2 (tools)
- Which tools and data sources are best for demand research and for bestseller research?
- Which platforms expose sales or ranking data, and what may be automated?
- Claude vs Perplexity vs other tools for market analysis: compare on real tasks.
