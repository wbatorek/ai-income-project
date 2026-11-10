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
- **R2a Public sales signals.** Collect sales counters, review counts, ranks and creator revenue posts
  per marketplace (e.g. ThemeForest, Notion template stores, Gumroad/Whop pages), with date and source,
  so trends can be measured over time. [C 03a] [R]
- **R2b Intrinsic vs borrowed value.** Tag each bestseller: did it sell because of the product
  (intrinsic) or the creator's audience (borrowed)? Only intrinsic-value bestsellers are templates for
  faceless products; borrowed-value ones point to partner opportunities. [C 03a]
- **R2c Creator-level bestsellers.** For each niche, record what comparable creators already sell, at
  what price and on which platform (Stan, Beacons, Whop, Gumroad, Kajabi). [C 03b]
- **R1b Audience questions as demand.** Recurring questions and complaints aimed at an account or
  community (comments, DMs shared by a partner, threads) are a primary demand signal. [C 03a] [C 03b]
- **R4b Pre-sale as proof.** Optional pre-sale or waitlist before full creation, behind an operator
  gate. [C 03a]
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
- **R10 Formats.** Format is a scored choice, not a fixed default. Ebook/PDF is the fastest topic
  test; **templates, trackers and planners** are the strongest faceless format (actively used) and come
  early; video (slides + AI voiceover, no avatars) later; chatbots over a corpus ("digital minds") only
  in phase 3. **Coaching/1:1 is out of scope** (fails the stop test). [C 03a]
- **R9b Creator-sourced synthesis.** In partner mode, build the product from the partner creator's
  content (with permission) plus external sources; the creator approves the final product. [C 03b]
- **R11 Quality.** Products must be good enough to avoid refunds and platform bans for low-quality
  AI content. [R]

### Distribution and sales (updated after Episode 3)
Three channels, compared by cost per sale and operator time [C 03a] [C 03b]:
1. **Partner channel (the course's main method).** Partner with micro-creators (10k–100k followers)
   who have a trusting audience but no product; we build the product, they promote it, revenue is
   shared (course: 50/50 "not uncommon", guests 17–50%). Creator first, product second. Only partly
   automatable: replies, calls, contracts and launches need the operator.
   - **R12a-1 Creator discovery** only through permitted means (official APIs, licensed creator
     databases, operator-assisted search). No scraping against platform terms.
   - **R12a-2 Qualification score.** Course filters as defaults (a video with 50k–200k views,
     10k–100k followers, no own product, business email) plus engagement quality, audience language and
     country, fit with a demand pocket, fake-follower check, and a credential check in health, finance
     and psychology niches.
   - **R12a-3 Outreach with approval.** The system drafts personalised emails; the operator approves the
     template and each batch; low volume, opt-out, suppression list; CAN-SPAM, GDPR/ePrivacy, PECR.
   - **R12a-4 Pipeline.** Found → qualified → contacted → replied → call → agreed → building →
     launched → reporting, with reply triage and drafted answers.
   - **R12a-5 Deal terms.** Lawyer-checked revenue-share template (split, term, IP, approvals,
     refunds, payouts). The operator signs.
   - **R12a-6 Launch kit.** Posts, stories, scripts, emails, FAQ and calendar for the creator to
     approve. The course didn't teach launches: research needed.
   - **R12a-7 Partner reporting.** Shared sales view per partner.
   - **R12a-8 Saturation check.** Avoid creators already flooded by course buyers.
2. **Owned faceless channel.** Daily simple posts in a niche for months, then products for the audience
   that forms. Highly automatable (generate + schedule, operator approves), but slow. [C 03a]
3. **Marketplaces.** Places where buyers browse and search (template and ebook marketplaces), suited to
   intrinsic-value products. [C 03a]

- **R13 Delivery.** Merchant-of-record platform (sales tax and VAT), automated delivery, **split
  payouts or affiliate links per partner**, attribution per creator (link or coupon), refunds, payouts
  to our country, and a fallback for **payment-account freezes**. Whop fees were never stated by the
  course: compare platforms. [C 03b] [R] [tax/]
- **R14 Feedback.** Track sales, refunds and reviews per product and per channel/partner, and feed
  results back into research and scoring. [R]

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
- Creator discovery: official APIs (Instagram Graph Business Discovery, YouTube Data API, TikTok) vs
  licensed databases (Modash, HypeAuditor, Upfluence, Heepsy): data, legality, cost.
- Outreach: Claude-drafted emails via a sequencer (Instantly, Smartlead, lemlist) vs ListKit vs Gmail at
  low volume; deliverability; reply classification.
- Partner CRM (sheet, Notion, Airtable, HubSpot free); contracts and e-signature.
- Store: split payouts or affiliates, MoR, payout country, lowest fees (Whop vs Gumroad, Lemon
  Squeezy, Payhip, Stan).
- Bestseller data: which marketplaces expose sales counts, and how to collect them legally.
- Which tools and data sources are best for demand research and for bestseller research?
- Which platforms expose sales or ranking data, and what may be automated?
- Claude vs Perplexity vs other tools for market analysis: compare on real tasks.
