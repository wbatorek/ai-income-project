# System requirements (phase 1, living document)

What the AI digital-product system must do. Tools are **not** chosen here; that is phase 2
([roadmap](roadmap.md)). Every requirement cites its source: **[C]** course knowledge (with the session,
e.g. [C 04a]), **[O]** operator knowledge, **[R]** our research ([R SYS] =
[self-running-ai-system](../research/self-running-ai-system.md), [R MON] =
[monetise-vs-own-system](../research/monetise-vs-own-system.md)), **[I]** ideas backlog.

> **Status: draft v0.9 (11 Nov).** Episode 3–4 interpretations and the Monetise decision are merged in.
> Frozen as **v1** at the end of the research sprint ([roadmap](roadmap.md)); after that, changes go in the
> change log at the bottom.

## Goal
Make a lot of money selling digital products, with a system that researches, creates and sells
them mostly on its own, while the operator approves key decisions. [O]

## Decided
- **D-1 Build our own system; don't buy Monetise ($1,995) now.** Its tools are GUI apps with no API shown,
  so they can't run inside a self-running pipeline; year-1 cash cost is about the same as our own stack;
  buying the same tools and filters as thousands of others makes creator-pool saturation worse. Re-decide
  after 6 weeks of building and outreach, only if the triggers in [R MON] §8 hold. [O] [R MON] [I #2]

## Build first (MVP scope, in this order)
These deliver the core value Monetise sells. Phase 3 follows this order ([roadmap](roadmap.md#phase-3-build)). [R MON] §8
1. **Creator discovery and qualification with a saturation score** (R12a-1, R12a-2, R12a-8).
2. **Creator-personalised product pipeline**: ingest (with permission), voice guide, pocket and promise,
   synthesis with external sources, outline → draft → QA → branded PDF (R9, R9b, R11). Also builds faceless products.
3. **Outreach with approval**: drafted emails, operator-approved batches, low-volume sending, reply triage,
   pipeline tracking (R12a-3, R12a-4, R12a-9).
4. **Deal and launch kit**: lawyer-checked revenue-share template, launch kit, partner communication kit
   (R12a-5, R12a-6, R12a-10).
5. **Store listing with revenue share via API**, sales webhooks to the operator's phone, partner sales view
   (R13, R12a-7, R14).

Everything else (automated demand and bestseller routines, owned channel, marketplaces, localisation, video)
comes after the first partner launch or the first sale.

## Functional requirements

### Research: two layers [O] [I #1]
- **R1 Demand research.** Find what people need and look for: problems, pain, urgency, search
  demand, recurring questions, complaints. Output "profitable pockets" with evidence. [C] [O]
- **R1b Audience questions as demand.** Recurring questions and complaints aimed at an account or
  community (comments, DMs shared by a partner, threads, our own channel's followers) are a primary demand
  signal. In partner mode, mine one creator's audience: what they ask, which videos get unusual views. [C 03a] [C 03b]
- **R1c Market-by-market analysis.** Research and score every opportunity per **niche × country ×
  language**, not only globally or in English. Compare markets side by side (demand, supply, price
  level, purchasing power, payment methods, platform availability, creator density, our ability to check
  quality in that language) and recommend the specific markets to sell in. Localise validated products to
  further markets. [O] [C 04a] [I #10]
- **R2 Bestseller research.** Find what currently sells best: products, platforms, formats, prices,
  sales and review signals, trends over time. Which formats sell best *per niche* is measured here. [O] [C 03a]
- **R2a Public sales signals.** Collect sales counters, review counts, ranks and creator revenue posts
  per marketplace (e.g. ThemeForest, Notion template stores, Gumroad/Whop pages), with date and source,
  so trends can be measured over time. [C 03a] [R]
- **R2b Intrinsic vs borrowed value.** Tag each bestseller: did it sell because of the product
  (intrinsic) or the creator's audience (borrowed)? Only intrinsic-value bestsellers are templates for
  faceless products; borrowed-value ones point to partner opportunities. [C 03a]
- **R2c Creator-level bestsellers.** For each niche, record what comparable creators already sell, at
  what price and on which platform (Stan, Beacons, Whop, Gumroad, Kajabi). Creators selling 1:1 services
  prove their audience pays. [C 03b]
- **R3 Pattern extraction.** From bestsellers, extract the *idea* (niche × format × price ×
  positioning) and propose a new, better or more specific product. Never copy content, branding or
  design. [O]
- **R4 Combine layers.** Rank opportunities that have both demand and proof of payment, plus a gap
  we can fill. In partner mode: creator score × pocket demand × proof that similar audiences buy × our
  ability to build a credible product there. [O] [C] [C 03b]
- **R4b Pre-sale as proof.** Optional pre-sale or waitlist before full creation, behind an operator
  gate. [C 03a]
- **R4c Conservative forecasts.** Every revenue forecast is a **range**, net of platform fees and the
  partner's share (17–50%); partner launches use 0.05–0.5% of followers as buyers. The low end is 20–30% of
  the naive forecast (real launches landed at 20–25% of projection). Rank opportunities by expected value
  per operator hour, and record forecast vs actual per launch (R14). Never promise numbers in outreach.
  [C 03b] [C 04a]
- **R5 Market choice.** Prefer markets where buyers *don't* solve the problem with AI themselves.
  Don't default to the operator's own professions. [O]

### Selection and planning
- **R6 Scoring.** Score opportunities with an explicit, adjustable model (first draft:
  [niche-finding.md](niche-finding.md); the course's five unlocks: pain, worsening pain,
  transformation, specificity, speed). Test a few levels of specificity instead of assuming narrower is
  better; a large market raises the ceiling score, not the entry score. [C] [C 04a]
- **R7 Product promise.** Every candidate gets "I help [who] with [worsening problem] get
  [result] in [time]". [C]
- **R8 Portfolio and pricing.** Plan a portfolio and price ladder, and test prices including higher
  points (price changes perceived value). Expect early products to earn $0 and iterate. [C] [C 03a]
- **R8b Test budget.** Every product or channel test has a capped cost (operator hours and money), a kill
  date and a success threshold, set before it starts. Default: ≤ 6 operator hours, ≤ $50 cash, kill or
  rework 21 days after publishing without a first sale ([niche-finding §2.4](niche-finding.md)). The
  operator adjusts the defaults. [C 04b] [R SYS]

### Creation
- **R9 Synthesis.** Build products by synthesising many credible sources (course: 150+) into one
  step-by-step method, with references. [C]
- **R9b Partner products: three ways of making them.** Chosen per partner: (a) the **creator writes**, we
  package, publish and launch (least work, least quality control, weakest claim to a share); (b)
  **co-creation** from the creator's content plus external sources; (c) **we build** and the creator
  approves. Creator content is used only with permission; the creator approves the final product. The
  deal template (R12a-5) covers each mode. [C 03b] [C 04a]
- **R10 Formats.** Format is a scored choice, not a fixed default. Ebook/PDF is the fastest topic
  test; **templates, trackers and planners** are the strongest faceless format (actively used) and come
  early; video (slides + AI voiceover, no avatars) later, also for higher-priced partner programmes;
  chatbots over a corpus ("digital minds") only in phase 3. **Coaching/1:1 is out of scope** (fails the
  stop test). [C 03a] [C 03b]
- **R11 Quality.** Products must be good enough to avoid refunds and platform bans for low-quality AI
  content. Covers, mockups and landing pages are generated but human-checked. No AI-written reviews or
  testimonials, ever; disclose AI assistance where a platform requires it. [R SYS] [C 03a]

### Distribution and sales
Three channels, compared by cost per sale and operator time [C 03a] [C 03b]:
1. **Partner channel (the course's main method, built first).** Partner with micro-creators (10k–100k
   followers) who have a trusting audience but no product; we build the product, they promote it, revenue
   is shared (course: 50/50 "not uncommon", guests 17–50%). Creator first, product second. Only partly
   automatable: the bottleneck is relationships, not production. [C 03b] [C 04a]
   - **R12a-1 Creator discovery** only through permitted means (official APIs, licensed creator
     databases, operator-assisted search). No scraping against platform terms. Store public metrics with
     date and source.
   - **R12a-2 Qualification score.** Course filters as defaults (a video with 50k–200k views,
     10k–100k followers, no own product, business email) plus engagement quality, audience language and
     country, fit with a demand pocket, fake-follower check, and a credential check in health, finance
     and psychology niches. The size band is adjustable (guests succeeded at 2–3k and at 5M).
   - **R12a-3 Outreach with approval.** The system drafts personalised emails (what we noticed, the
     specific product idea, no-upfront-cost revenue share); the operator approves the template and each
     batch; low volume, opt-out, suppression list, sending-domain hygiene; prefer the creator's published
     business channel; CAN-SPAM, GDPR/ePrivacy, PECR.
   - **R12a-4 Pipeline.** Found → qualified → contacted → replied → call → agreed → building →
     launched → reporting, with reply triage and drafted answers. Record the source, including
     **referrals** ("introduced by partner X"). Plan for a slow first partner (the guest's second came
     ~1.5 months after the first). [C 04a]
   - **R12a-5 Deal terms.** Lawyer-checked revenue-share template: split, term, exclusivity, IP, who
     makes the product (R9b mode), content approval, refunds and support, what happens if promotion stops,
     payouts and tax forms. The course gave only one example (30/70 + $6k upfront, WB3): research needed.
     The operator signs.
   - **R12a-6 Launch kit.** Named copy pieces, each approved by the operator and then the creator:
     talking points for the creator's posts, post and story copy, video scripts, email sequences, product
     and sales page copy, FAQ, and a launch calendar. The same pieces, adapted, for the owned channel and
     marketplaces. Written by Claude with a per-partner voice guide (no Ghostwriter OS). The course didn't
     teach launches: research needed. [C 04b]
   - **R12a-7 Partner reporting.** Shared sales view per partner, with the forecast **range** (R4c)
     next to actuals.
   - **R12a-8 Saturation check.** Before contacting a creator, score saturation from: (1) course-path
     overlap: high rank for the course's "industry + tips" Instagram search in fitness, parenting,
     relationships or money; (2) a rising share of similar creators in the cohort with a new Whop/Stan link
     (R2c data); (3) our falling reply rate per niche and language (R12a-4); (4) creator posts about being
     pitched product deals. Prefer less obvious entry points: YouTube, TikTok, Telegram, podcasts,
     newsletters, niches outside the big three, non-English markets (R1c). [C 04a]
   - **R12a-9 Partner cap.** A maximum number of active partners set from the operator's weekly hours
     (start with 1–3); the system tracks operator time per partner and warns before the cap is hit. [C 04a]
   - **R12a-10 Partner communication.** Drafted status updates, next steps, positioning rationale, launch
     debriefs and an FAQ for each creator, approved by the operator. Expectation-setting and reassurance
     stay human. [C 04a]
2. **Owned faceless channel.** Daily simple posts in a niche for months, then products for the audience
   that forms. Highly automatable (generate + schedule, operator approves), but slow. Follower questions
   feed R1b. [C 03a]
3. **Marketplaces.** Places where buyers browse and search (template and ebook marketplaces), suited to
   intrinsic-value products. [C 03a]

- **R13 Delivery.** Merchant-of-record platform (sales tax and VAT), automated delivery, **split
  payouts or affiliate links per partner**, attribution per creator (link or coupon), refunds, payouts
  to our country, instalments/subscriptions, local payment methods in target markets (R1c), and a second
  platform ready as a fallback for **payment-account freezes**. Whop fees were never stated by the
  course: compare platforms. [C 03a] [C 03b] [R] [tax/](../tax/)
- **R14 Feedback.** Track sales, refunds, reviews and buyer questions per product and per
  channel/partner, plus forecast vs actual (R4c), and feed results back into research and scoring. [R]
  - **R14b Concentration check.** Report the revenue share per platform, channel and partner; warn when
    one exceeds 60% (adjustable) and keep the R13 fallback ready. [C 04b]
  - **R14c Improvement loop.** Every live product gets a scheduled review (sales, refunds, reviews, buyer
    questions) ending in a proposed change: improve, re-price, re-position or kill. Ideas can be copied;
    our edge is iteration speed and quality. [C 04b]

### Operator control
- **R15 Approval gates.** The operator approves: entering a niche, publishing, public posting, any
  spending, prices, partner deals. Nothing happens without a decision. [O] [R]
  - **R15b Decision deadlines.** Every approval request carries a recommendation, the downside if it
    fails, the cost of waiting, and a deadline with a default (usually "no"), so nothing stalls in
    "I'll think about it". [C 04b]
- **R16 Transparency.** Every recommendation shows its evidence and sources.
  - **R16b Research stopping rule.** Every research run states the decision it informs, the evidence
    threshold and a budget (time, tokens, money). It stops when the threshold is met or the budget is spent
    and reports "what we still don't know". This applies to our own phase 1 too ([roadmap](roadmap.md)). [C 04b]

## Non-functional requirements
- **N1 Mostly autonomous**, with a low weekly time cost for the operator (target: under 2 h a week for
  approvals; partner relationship time is capped separately by R12a-9). [O] [R SYS]
- **N2 Cost-aware, no fixed costs before sales.** Use the existing Claude Ultra subscription where it
  fits; add paid tools only when they're clearly better for a job. Until a product has sold: no paid ads,
  inventory, annual contracts or upfront partner fees; monthly, cancellable plans and trials only. Every
  recurring cost needs operator approval (R15). [O] [C 04a] [C 04b]
- **N3 Legal.** Respect platform terms of service, copyright, privacy (creator data) and tax rules. [R]
- **N4 Best tool per job.** Claude isn't assumed to be best at everything (e.g. market analysis
  might be better with Perplexity or data tools). Decided in phase 2. [O] [I #3]
- **N5 Safe by design.** Spend caps, a `PAUSED` kill switch every job checks, least privilege (agents
  that read the web can't publish, pay or post), no community posting credentials for agents, scraped text
  treated as data, idempotent webhooks. [R SYS] §5.5

## Phase 2 decisions
The tool decisions, options and criteria are in [roadmap.md › Phase 2](roadmap.md#phase-2-tools). The
research sprint ([roadmap.md › Research sprint](roadmap.md#research-sprint-wed-11-nov-about-3-hours)) answers
the open questions behind them (creator data, outreach, store, bestseller and demand data per country).

## Change log
- **11 Nov, v0.9:** added D-1 and the build-first list (Monetise decision); R4c forecasts, R6 specificity
  tests, R8b test budget, R9b three modes, R11 visuals and reviews, R12a-4 referrals, R12a-6 named copy
  pieces, R12a-7 forecast range, R12a-8 concrete signals, R12a-9 partner cap, R12a-10 partner communication,
  R13 instalments and fallback, R14b concentration, R14c improvement loop, R15b deadlines, R16b stopping
  rule, N2 no fixed costs before sales, N5 safety. Phase 2 questions moved to the roadmap.
