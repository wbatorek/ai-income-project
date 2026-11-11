# Roadmap: from research to a running pipeline, fast

*Our plan, 11 Nov 2026. Dates are Thailand time. Requirements: [requirements.md](requirements.md) (IDs below refer to it).*

The operator wants to build **this week**, not in a few weeks. So phase 1 ends with one parallel research
sprint and a hard stop (R16b applied to ourselves). Anything still unknown after that becomes an experiment
in phase 3, not more research.

| When | What | Done when |
|---|---|---|
| **Wed 11 Nov** | Research sprint: 7 parallel agents (~3 h), operator reads the summaries (~45 min) | 7 reports in `research/` |
| **Thu 12 Nov** | Synthesis: market shortlist, requirements frozen as v1 | Phase 1 stopping rule met |
| **Fri 13 Nov** | Phase 2: tool decisions (half a day, with sign-ups and trials) | `system/tools.md` filled, G5 approvals given |
| **Sat 14 Nov →** | Phase 3: build in the "build first" order | Steps 0–2 working by Thu 19 Nov |
| Mon 16 Nov | Finale and Episode 4 part 2: processed as a **delta** only, doesn't block the build | Changes logged in requirements |
| **Sat 26 Dec** | 6-week checkpoint: continue or kill per channel (R8b); Monetise re-decided only if the [§8 triggers](../research/monetise-vs-own-system.md#8-recommendation) hold | Written decision |

---

## Research sprint (Wed 11 Nov, about 3 hours)

**Setup (15 min).** One agent per task, all started at once. Earlier sessions couldn't open vendor pages
(whop.com, docs.whop.com, gumroad.com, listkit.io, reddit.com, etsy.com), so either allow those hosts first or
mark such facts **[unverified]**. Every report has the same shape: a 10-line summary; a decision table with a
recommendation and confidence; prices with date and source; legality and terms of service; "what we still don't
know"; the requirement IDs it informs. Every agent stops at its evidence threshold or after 3 hours (R16b).

**S1. Other systems and teachers** → `research/other-systems.md` (2 h). Who else runs or teaches
digital-product businesses, beyond Iman: (a) creator-partnership models: the Russian-speaking "producer"
(продюсер) model the course's guests came from, done-for-you creator-product agencies; (b) faceless template and
marketplace sellers (Notion, Etsy, Gumroad); (c) AI-run product businesses (e.g. Nat Eliason's Felix). For each:
method, unit economics, what they automate, evidence quality, what to copy and what to avoid. Stop at 8–12
well-evidenced models. Informs idea #4, R9b, R10, R12a.

**S2. Bestseller data per platform and country** → `research/bestseller-data-sources.md` (2–3 h). For each
marketplace (Gumroad Discover, Etsy, Envato/ThemeForest, Notion Marketplace, Whop Discover, Payhip, Stan/Beacons
storefronts, Amazon KDP, Udemy, plus local marketplaces in candidate markets): which sales signals are public
(counters, reviews, ranks), per country and language, whether an API or allowed access exists, third-party tools
(EverBee, eRank, Publisher Rocket) and their cost. Output: a source matrix ranked by signal quality × legality ×
cost, and the 3 sources to automate first. Informs R2, R2a–c, R1c.

**S3. Demand data per country and language** → `research/demand-data-sources.md` (2–3 h). Keyword volume per
country and language (Google Ads Keyword Planner, DataForSEO, Semrush/Ahrefs), Google Trends API access, YouTube
Data API (region and language filters), Reddit API status, local forums and Facebook groups, Telegram channel
analytics, marketplace reviews as complaint mining. Include a side-by-side test: the same pocket question in two
languages to Claude (Ultra research) and Perplexity Pro. End with a **first shortlist of 3–5 niche × country ×
language markets** with purchasing power and platform/payment availability. Informs R1, R1b, R1c, N4, idea #3.

**S4. Creator discovery: data sources and legality** → `research/creator-discovery.md` (2–3 h). Instagram Graph
Business Discovery (what it returns, requirements, rate limits), YouTube Data API, TikTok APIs (eligibility),
Telegram, podcasts and newsletters; licensed databases (Modash, HypeAuditor, Heepsy, Upfluence, influencers.club):
coverage of non-English creators, audience country and language, fake-follower data, email availability, price,
monthly trials. Legal basis for storing creator business emails (GDPR legitimate interest, country specifics).
How to measure the R12a-8 saturation signals. Output: a recommended discovery stack for 1 niche × 2 markets and the
cost per 100 qualified creators. Informs R12a-1, R12a-2, R12a-8.

**S5. Outreach tooling and deliverability** → `research/outreach-tooling.md` (2 h). Instantly vs Smartlead vs
lemlist vs plain Google Workspace at 20–50 emails a day: domains and mailboxes (SPF, DKIM, DMARC, warm-up time),
email verification, an API to push Claude drafts and pull replies for triage. DMs as an alternative channel and
their platform rules. Cold-email rules for sole-trader creators by country (GDPR/ePrivacy, Germany's UWG, UK PECR,
US CAN-SPAM). Pipeline CRM (sheet, Airtable, Notion, HubSpot free) and e-signature. Output: a setup checklist with
monthly cost and a compliance rule per target country. Informs R12a-3, R12a-4.

**S6. Launch formats and deal terms for creator partnerships** → `research/launch-and-deals.md` (3 h). The course
skipped both. Launches for 10k–100k creators: story sequences, lives and webinars, challenges, waitlist plus
pre-sale, broadcast channels, email sequences, Telegram launches, evergreen after launch; timelines, real
conversion rates with sources, and which copy pieces each needs (R12a-6). Deal terms in the market: split ranges,
upfront fees, term, exclusivity, IP, who makes the product (R9b modes), refunds, ending the deal; where to get a
lawyer-checked template and what it costs. Output: **one default launch playbook and one default term sheet**,
ready to become templates. Informs R4c, R9b, R12a-5, R12a-6, R12a-7, R12a-10.

**S7. Delivery platforms with split payouts** → `research/delivery-platforms.md` (2 h). Whop vs Gumroad, Lemon
Squeezy / Stripe Managed Payments, Payhip, Stan, Paddle, Podia/Kajabi, Stripe Connect: merchant of record and
VAT/sales tax coverage, all-in fee on a $49 international card sale, native split or affiliate commission per
partner, attribution, payouts to our US LLC ([tax/](../tax/)), API (create product, upload file, webhooks),
instalments, local payment methods in target markets, account-freeze record, how to leave. Output: a primary and a
fallback platform. Informs R13, R12a-7, R14b.

---

## Phase 1 end: stopping rule

**We know enough when:**
1. The 7 sprint reports exist, and every phase 2 decision below has at least two priced, legal candidates and a
   recommendation.
2. The operator has approved (G1) a **start shortlist: 1–2 niches × 1–2 markets** (country × language), each with a
   rough demand signal, a bestseller signal and a creator-pool estimate.
3. A default launch playbook and term sheet exist (the lawyer check happens in phase 3).
4. `requirements.md` is frozen as v1, and every remaining unknown is written as a "learn by doing" item with a date.

**We don't wait for:** the Finale or Episode 4 part 2, the contents of Monetise's playbook, verified market sizes, or
perfect data.

**Target: Thu 12 Nov 2026, end of day. Hard stop: Fri 13 Nov, noon.**

---

## Phase 2: tools

**Fri 13 Nov, half a day.** Criteria, in order:
1. Meets the requirement IDs.
2. Automation is legal and within the terms of service.
3. Has an API, so it can run inside the pipeline instead of as a manual click-step.
4. Monthly, cancellable, with a free tier or trial; nothing annual before sales (N2).
5. Easy to leave.
6. Wins a quick real test where quality matters.

Pick the cheapest option that passes 1–3.

| # | Decision | Options | Decided by |
|---|---|---|---|
| T1 | Runtime and scheduling | Claude Code routines + repo files (MVP) / Agent SDK scripts / n8n | Run caps on Ultra, can it commit to the repo, approval fit |
| T2 | State and approvals | Files + `system/approvals/queue.md` / SQLite + Telegram bot | Time to build, approving from a phone, audit log |
| T3 | Research tools | Claude Ultra / + Perplexity Pro / + DataForSEO or Keyword Planner | S3 test, country-level data, cost per run |
| T4 | Creator discovery | Official APIs / + one licensed database for 1 month | S4: coverage in our markets, legality, cost per qualified creator |
| T5 | Outreach and CRM | Sequencer or Workspace + domains + verifier; sheet or Airtable | S5: deliverability, API, compliance, price |
| T6 | Store and payouts | Whop / Gumroad / Payhip / Stan / Paddle, plus a fallback | S7: MoR, all-in fee, split, payouts to the LLC, API, freeze record |
| T7 | Rendering and design | Typst / HTML + Playwright / Canva; Notion or Sheets templates | Quality of one sample, automation |
| T8 | Contracts | Template source + lawyer check + e-signature | S6: cost, jurisdiction |

**Output:** `system/tools.md` (choice, reason, cost per month, cancel-by date). Each paid item goes through G5 with
a deadline (R15b). **Buy the sending domains on the same day:** warm-up takes about 2–3 weeks [est.].

---

## Phase 3: build

**From Sat 14 Nov.** The order follows "Build first" in [requirements.md](requirements.md#build-first-mvp-scope-in-this-order).
Each step ends with something usable and an operator gate. Dates are targets.

| # | Build | Operator gate | Target |
|---|---|---|---|
| 0 | **Skeleton:** folders and state files, approval queue with deadlines and defaults (R15b), `PAUSED` switch, spend log, research-run template with a stopping rule (R16b) | None | Sat 14 Nov |
| 1 | **Creator discovery and qualification** for the shortlist, with a saturation score (R12a-1, -2, -8) | G1: niche and market, creator shortlist | Mon 16 Nov |
| 2 | **Product pipeline:** ingest → voice guide → pocket and promise → synthesis → outline → draft → QA → branded PDF (R9, R9b, R11). Also builds faceless products | G2: quality sign-off | Thu 19 Nov |
| 3 | **Outreach with approval:** drafts → batch approval → sending → reply triage → pipeline, within the partner cap (R12a-3, -4, -9) | Template and every batch | First 10–20 emails ~Sat 21 Nov; volume rises with domain warm-up |
| 4 | **Deal and launch kit:** term sheet with lawyer check, launch kit with named copy pieces, partner communication kit, forecast ranges (R12a-5, -6, -10, R4c) | Operator signs; G5 for lawyer cost; creator approves | By the first "interested" reply (~end of Nov) |
| 5 | **Store listing with revenue share via API** (hidden until approved), sales webhooks → phone alerts, partner sales view (R13, R12a-7) | G3: publish and price | Before the first launch |
| 6 | **Feedback:** weekly report, forecast vs actual, concentration check, improvement loop (R14, R14b, R14c) | Operator approves changes | After the first sale |

**Later:** automated demand and bestseller routines (R1–R4), owned faceless channel, marketplace channel,
localisation to further markets, video formats.

**Parallel track (operator decision, recommended):** a small real test. Build one ebook or template MVP with step 2
and sell it through step 5 on one marketplace or channel, capped by R8b (a few evenings, no fixed costs). The first
partner usually takes weeks, so this gives the system real sales data in the meantime ([C 04a](../course/sessions/04a-vip.md), [C 04b](../course/sessions/04b-main.md) §6).
