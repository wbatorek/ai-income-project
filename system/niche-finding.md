# Niche finding and product planning (design v1)

*Our design, 9 Nov 2026. It uses course knowledge and our own research, and cites both so you can tell
them apart. It replaces the two draft scoring models in the session notes.*

**Source codes used below**

| Code | File | Kind |
|---|---|---|
| [KB] | [course/knowledge/README.md](../course/knowledge/README.md) | Course |
| [CP] | [course/knowledge/choosing-products.md](../course/knowledge/choosing-products.md) | Course |
| [BP] | [course/knowledge/buyer-psychology.md](../course/knowledge/buyer-psychology.md) | Course |
| [PT] | [course/knowledge/product-types.md](../course/knowledge/product-types.md) | Course |
| [DV] | [course/knowledge/develop.md](../course/knowledge/develop.md) | Course |
| [S02a] / [S02b] | [02a §10](../course/sessions/02a-vip-choosing-products.md), [02b §10](../course/sessions/02b-develop.md) | Our interpretation of the course |
| [SYS] | [research/self-running-ai-system.md](../research/self-running-ai-system.md) | Our research |
| [IDEAS] | [research/product-ideas-own-expertise.md](../research/product-ideas-own-expertise.md) | Our research |

---

## 1. Purpose and principles

**Purpose.** Every week, the system turns a few seeds into a short ranked list of product
opportunities. Each one comes with evidence, a score, a product promise and a price. The operator
then only has to say yes or no. Nothing gets built without that yes (gate G1).

**Course rules we follow**

| Rule | Source |
|---|---|
| Start from demand, not passion. A pocket is a problem people **already search for, already pay for, and can't solve well yet** | [CP] §2, §5.1 |
| A pocket is a specific person with a specific problem, narrowed by a real trait (not "busy"), but still common | [CP] §3 unlock 4, §5 |
| Score on the five unlocks: pain, worsening pain, transformation, specificity, speed | [CP] §3 |
| Pain, not pleasure. Wealth, health and relationships first. Reminder frequency measures pain | [CP] §3, [BP] §2 |
| Every opportunity must fit the four-part promise: "I help [who] with [worsening problem] get [result] in [time]" | [CP] §4 |
| Generate well past your first ideas. Then rank, and pick the highest | [CP] §2, §6 |
| Start with the simplest format (ebook or digital asset). Add complexity only after sales | [PT] §3.2, [DV] §4 |
| Iterate as a portfolio. Expect $0 from the first products, and keep the earners | [DV] §6 |
| Put the product where presold buyers already gather (groups of 10k–100k) | [KB] rule 15, [BP] §1 |

**Our additions**

| Addition | Source |
|---|---|
| **Evidence first:** every score points to URLs in an evidence pack (the course's tool showed a /10 score with no visible data) | [S02b] §5.3 |
| Demand proof (searched + paid) is a hard gate | [S02b] §10.1 |
| **Warm access to buyers** (new criterion R2): for a first sale, an audience you already have beats raw score | [IDEAS] §4, [SYS] §6 |
| Gates on operator verifiability and on policy/platform risk (AI-slop crackdowns, Etsy's 22 Oct 2026 ban on AI guides) | [SYS] exec. #6, §4, §5.2 |
| Code controls the pipeline, state lives in files, nothing moves without a decision | [SYS] §1 |
| Automate data collection only where terms allow; the rest is a manual checklist | [SYS] §3.1, §5.1 |
| Kill rules and a learning loop | [SYS] exec. #10, [S02b] §10.4 |

---

## 2. Scoring model v1

### 2.1 Formula

Each criterion is scored 1–5 by the scoring agent. Each score has a one-line reason, a confidence
level and evidence references. **Code, not the LLM**, works out the total and applies the gates:

`score = Σ(criterion score × weight) / 5`. The result runs from 20 to 100. We keep `/5`, as in
[IDEAS], so the 30 existing scores stay comparable.

The weights are stored in `system/scoring/weights-v1.json`. Desirability (the course's five
unlocks) is 45%, market proof 26%, access to buyers 17%, and build and risk 12%.

### 2.2 Criteria and rubrics

| # | Criterion | W | 1 | 3 | 5 |
|---|---|---|---|---|---|
| D1 | **Pain intensity**, measured by reminder frequency | 15 | Pleasure or want, rarely felt | Real pain, felt weekly | Felt daily. Blocks work, money or sleep |
| D2 | **Worsening and urgency** | 9 | Static | Gets worse over months | Escalates in days or weeks, or there's a hard deadline (go-live, end of support, penalty date) |
| D3 | **Transformation clarity** | 8 | Vague ("be better at X") | B is stated but hard to observe | Point A (feel, fear, avoid, self-image) and an observable point B, mapped from buyers' own words |
| D4 | **Specificity, with enough people** | 8 | Generic or fake-specific (the qualifier fits more than 80% of the base group) | One real distinguishing trait | A trait plus a specific problem, and plausibly 5,000 or more people have it |
| D5 | **Speed** (credible and time-bound) | 5 | No time frame, or an unbelievable one | Months | Days to two weeks, in line with what competitors promise |
| M1 | **Demand proof: searched + paid** | 12 | No evidence of either | Both: ≥ 3 independent search or ask signals **and** ≥ 1 paid solution to this problem in any form (product, course, service, gig, tool) | Both strong: threads recurring for 2+ years or measured keyword volume, **and** visible traction for paid digital products in this segment |
| M2 | **Ability and willingness to pay** | 9 | Students or hobbyists, free alternatives everywhere | Consumers with a budget ($19–39) | Company card, or tied to money or career. The alternative costs 10× our price or more |
| M3 | **Solution gap** | 5 | A strong, specific incumbent at a similar price | Incumbents are free, scattered or generic | No product made for this segment. Incumbents are generic, slow, outdated or poorly rated, and threads go unanswered |
| R1 | **Reach** (open channels and partners) | 9 | Nowhere to reach them, or every community bans promotion | One community of 10k+ where value posts are allowed, or real SEO demand | Several 10k–100k communities, partner creators and marketplace search |
| R2 | **Warm access to buyers** *(new)* | 8 | The operator is unknown to these buyers | 10–30 direct contacts who are buyers or will forward it, or a real posting history in one buyer community | An owned audience of 1k+ in the segment, or a committed partner placement or pre-orders (4 = 30+ direct contacts in the buyer role) |
| B1 | **Operator verifiability** | 6 | The operator can't fact-check it | He can check it with effort | It's his own expertise, and he can test every claim |
| B2 | **Evidence base** (enough sources to synthesise) | 2 | No credible sources | Official docs or reputable sources are enough | Official specs plus the operator's own tested material, or 50+ credible sources |
| B3 | **Production effort** | 2 | Needs video or an app before the first sale | 5–7 days with about 4 h of operator review | 2–4 days. A PDF or template the agent drafts and the operator tests |
| B4 | **Policy and claim risk** | 2 | Medical, legal, financial-guarantee or minors' safety outcomes, or the target channel bans it | The promise depends on a third party's judgment, or the topic is tax- or legal-adjacent | Neutral, checkable claims |

**R2 data** comes from `system/operator-profile.md`, a list the operator keeps of networks and
rough contact counts per buyer role. It holds **counts only, no names**, because this is personal
data under the GDPR. The agent proposes R2. The operator confirms it at G1.

### 2.3 Hard gates (reject regardless of total)

| Gate | Rule | Source |
|---|---|---|
| Pain | D1 < 3 | [CP] §3, [S02a] |
| Specificity | D4 < 3, which includes the fake-specificity check | [CP] §3 |
| **Demand proof** | M1 < 3: no proof that people **both** search for it **and** pay for it. If an evidence source was blocked, the item gets **one** manual evidence task (`needs_evidence`) and is then re-scored or rejected | [CP] §5.1, [S02b] §10.1 |
| Access | max(R1, R2) < 3: no route to any buyer | [KB] rule 15. EDI kit case, [IDEAS] top 5 |
| Verifiability | B1 < 3 | [SYS] §5.2 |
| Evidence base | B2 < 2 | [S02b] §10.2 |
| Policy | B4 = 1 | [SYS] §5.2, §4 |

### 2.4 Thresholds

**Before building**

| Score (all gates pass) | Status | Next step |
|---|---|---|
| ≥ 75 | `recommend` | Goes into the ranked plan for G1 |
| 65–74 | `cheap_test` | Into the plan only if it builds in ≤ 5 days with ≤ 4 h of operator review |
| 55–64 | `needs_evidence` | One more evidence cycle, then re-score or drop |
| < 55, or any gate fails | `rejected` | The reason is logged in `research/niches/index.json` |

Scores less than 2 points apart count as a **tie**, because the 1–5 inputs are noisy. Ties go to the
planning agent's tie-breaks (§4).

**After launch** (combines [SYS] §7 and [S02b] §10.4)

The test window is **21 days**. Minimum exposure: 5 approved value posts in at least 2 channels, or 1
partner placement, plus outreach to 20 or more warm contacts if R2 ≥ 3. Every channel gets its own
tracking link.

| Signal | Diagnosis | Action |
|---|---|---|
| Under 100 landing visits | A distribution problem, not a verdict on the product | Extend 14 days with new channels, **once** |
| 100+ visits and 0 sales | The pocket or the promise is wrong | Reposition the promise once, otherwise **kill** |
| Conversion under 1% | Packaging or price | Change title, cover, price or offer (G3) |
| Refunds over 5%, or 2 refunds with the same reason | Quality | Stop distribution and revise the content (G2) |
| 7-day average of $15/day or more ([DV] §6) | It works | Scale: next tier on the ladder, adjacent pockets |

**Learning loop.** Every launch writes its score and outcome to `index.json`. After 10 launches the
analytics agent proposes new weights. The operator approves them, and they become `weights-v2.json`.

### 2.5 How the course contradictions are resolved ([KB] table, [CP] §7)

| Contradiction | v1 resolution | Where in the model |
|---|---|---|
| "No digital products sold" vs "already paying" | **Proof that people pay for the general problem, but no good *specific* product for this segment.** Zero competitors means *low* M1, not high M3 | M1 gate, M3 |
| A few dozen vs a few hundred vs millions of buyers | We need a pool that can produce about 100+ sales: 5,000+ people with the problem (D4), reachable through at least one route (access gate). Beyond that, size isn't rewarded | D4, R1 |
| Weight loss is weak vs it's a model pocket | Score the *narrowed* pocket, never the broad topic. A deadline plus an identity trigger (postpartum) can lift D1 and D2. Health is still capped by B4 | D1, D2, D4, B4 |
| Simple, obvious ideas vs "first ideas are your worst" | Generate 30 pockets per seed, so we go past the obvious ones. **Reward proven demand, not novelty.** In short: a simple problem in a non-obvious segment | Stage S1, M1 |
| "The market doesn't care about your passion" vs "enter your skill" | Passion is never scored. The operator's skill counts only through what it does for buyers: quality (B1) and access (R2). The demand gates still apply | B1, R2 |
| "Pain is 90%" vs "the pocket is half the way" | D1 has the highest weight and a gate, but not 90%: that number is rhetoric, not data ([BP] §7 note) | D1 |
| 1–20 pages vs ~45 pages; build in minutes vs Michal's 2–4 days | Length is not scored. B3 rewards the shortest asset that reaches point B, measured in real build days plus operator review hours | B3, §4 |
| "The solution doesn't matter" vs 150 references | We side with quality: gates on B1 and B2, plus QA at G2 | B1, B2 |
| "Nobody googles 'buy golf ebook'" vs "what people search for" | People search for the *problem* (M1). They buy where they gather (R1, R2). Both are needed | M1, R1/R2 |
| 4 vs 5 formats; Whop "free" vs a fee | Neither affects the score. The planning agent uses our own format list and **net** prices after fees | §4 |

---

## 3. Pipeline

```
S0 seeds → S1 pockets → S2 evidence packs → S3 scoring → S4 promise + plan → ✋ G1 → S5 hand-off → product creation
```

### 3.1 Stages

| Stage | Agent / model | Inputs | Outputs | Cost per week |
|---|---|---|---|---|
| **S0 Seed generation** | Research agent (Sonnet) | `operator-profile.md` (skills, networks); deadline watchlist (official EOL and regulatory dates); learnings from `index.json` (adjacent pockets of earners); course pillars | `research/seeds/YYYY-Www.md`: 3–5 seeds, each tagged *expertise / deadline / adjacent / open* | ~$0.20 |
| **S1 Pocket discovery** | Research agent (Haiku generates, Sonnet filters) | Seeds, plus `index.json` for duplicates | `research/pockets/YYYY-Www.json`: 30 "person + problem" pockets per seed, with the fake-specificity check and a no-web pre-screen on D1, D4, B1 and B4. **The top 8 go on to S2** | ~$0.50 |
| **S2 Evidence collection** | Research agent, one subagent per source family (Sonnet; Haiku tags the quotes) | Top 8 pockets | `research/niches/<slug>/evidence.json` + `evidence.md` (schema below), including `manual_checks` for the operator | ~$1 per niche, ~$8 |
| **S3 Scoring** | Scoring agent (Opus). **It reads only the evidence pack, with no web access**, which limits prompt injection. Then a red-team pass (Sonnet) writes "why it might fail" | Evidence packs, rubric, weights | `research/niches/<slug>/score.json` (criterion scores, reasons, confidence, refs). `scripts/score.py` adds the total, gates and status | ~$0.30 per niche, ~$3 |
| **S4 Promise and plan** | Product-planning agent (Opus) | Niches scoring ≥ 65 with all gates passed, plus the portfolio | A/B map, promise, format, price and ladder slot per niche. `products/plan/YYYY-Www.md` + `plan.json`. New items in `system/approvals/queue.md` | ~$2 |
| **✋ G1** | Operator | Queue entries | `decision:` lines, logged to `system/approvals/decisions.jsonl` | 15–20 min of operator time |
| **S5 Hand-off** | Orchestrator script, no LLM | Approved items | `products/<slug>/` with `idea.md` (promise, A/B), `validation.md` (link to the evidence pack and score), `brief.md` (the creation brief) and `status.json` = `approved_for_creation` | $0 |

**Total: about $15 a week, roughly $60 a month**, plus about 1–1.5 h a week of operator time
(manual checks plus G1). That's inside the $30–150 a month in [SYS] §2. The token prices used here
come from [SYS] §2. Web search is assumed at about $10 per 1,000 searches *[check current pricing]*.

### 3.2 Evidence pack (one per niche)

```json
{
  "slug": "netsuite-saved-search-formulas", "week": "2026-W48", "seed": "expertise:netsuite",
  "pocket": {"who": "NetSuite admins and finance power users", "trait": "own the report queue",
             "problem": "saved-search formulas throw 'Invalid Expression'", "pillar": "wealth/career"},
  "demand": {
    "searched": [{"signal": "forum thread", "url": "…", "date": "2025-03", "note": "unresolved"}],
    "paid":     [{"type": "service|product|course|tool|gig", "url": "…", "price": "…", "traction": "…"}],
    "unsolved": [{"quote": "…", "url": "…"}]
  },
  "quotes":       [{"text": "…", "url": "…", "tags": ["daily", "deadline"]}],
  "segment_size": [{"proxy": "r/Netsuite members", "value": 29000, "source": "…", "as_of": "…"}],
  "channels":     [{"name": "…", "members": 0, "promo_rules": "allowed|value-only|banned|unverified", "url": "…"}],
  "partners":     [{"name": "…", "audience": 0, "fit": "high|med|low"}],
  "incumbents":   [{"name": "…", "price": "…", "gap": "generic|slow|outdated|poor reviews"}],
  "source_base":  {"count": 0, "official": 0, "consensus": "high|mixed|low"},
  "warm_access":  {"proposed_r2": 4, "basis": "operator-profile: NetSuite clients and LinkedIn", "operator_confirmed": false},
  "manual_checks":   [{"task": "Google Trends 5y: 'netsuite case when'", "status": "todo"}],
  "blocked_sources": ["reddit.com fetch"],
  "cost_usd": 0.9
}
```

`evidence.md` is the same content written for a human: quotes, tables and links. Each pack needs at
least 5 verbatim quotes with URLs, 3–10 incumbents, and every channel's promotion rules (or
`unverified`).

### 3.3 Data sources and terms of service

| Source | Feeds | Access | Automate? |
|---|---|---|---|
| Claude web search / fetch of public pages | Quotes, incumbents, prices, channels | Built-in tool | **Yes**, at low volume. No logins. Respect robots.txt |
| Public forums (Audacity, Oracle community, NetSuite Professionals archive); Stack Exchange API | D1, D2, M1 (searched) | Public pages; official API with a free key | **Yes** |
| Reddit | Quotes, member counts | The API needs approval under the Responsible Builder Policy ([SYS] §3.1) | **No API, no scraping.** Search snippets only, and the operator browses the top threads |
| YouTube Data API v3 | Partner creators (R1), comment quotes | Official. 10,000 units a day; one search costs 100 | **Yes** |
| Etsy Open API v3 | M1 (paid): listings, prices, reviews | Official read access, 10k requests a day | **Yes**, read-only. We don't *sell* guides there |
| Gumroad, Whop, Udemy, Fiverr, Upwork public pages | M1 (paid), M3, price anchors | No bestseller APIs | Fetch individual pages at low volume, or check manually. **No mass scraping** |
| Amazon Kindle (search, Best Sellers Rank) | M1 (paid) | No free API | **Manual**, for the top 3 niches only. A paid tool needs G5 |
| Google Trends | D2 seasonality, M1 (searched) | The official API is alpha and by application. Scrapers break its terms | **Manual**, 2 min per niche. Apply for the API |
| Keyword volume (Keyword Planner, DataForSEO) | M1 (searched) | Licensed. Needs an Ads account or pay-per-call | Phase 2, after G5 spend approval. MVP: "People also ask" in search results plus manual Keyword Planner |
| Facebook groups, LinkedIn, Slack, Discord | Quotes, R1, R2 | No groups API. LinkedIn bans scraping. Slack and Discord are members-only | **Manual only.** Paraphrase private messages, never export members, store no personal data |
| Official docs, standards; PubMed, OpenAlex, Semantic Scholar, Crossref | B2 | Open | **Yes** |
| Own files (`operator-profile.md`, `portfolio.json`, sales) | R2, learning loop | Repo | **Yes** |

The research agent writes only to `research/`. Anything it reads from the web is data, never
instructions ([SYS] §5.5).

---

## 4. Product-planning agent

**Job:** turn scored niches into a **ranked, portfolio-balanced plan**. For each niche it decides
the format, the price and the ladder slot, writes the promise and the creation brief, and proposes
whether to keep, scale or kill live products (from analytics, once that agent exists). It never
spends money, publishes anything or changes prices. It only proposes.

**Inputs:**
- `score.json` and the evidence packs, for niches that are `recommend` or `cheap_test`
- `products/portfolio.json`: live products, cluster, channel, sales, refunds
- `operator-profile.md`: weekly hours, build capacity, verified domains
- platform notes: Whop fees, the Etsy and KDP rules ([SYS] §4)

### Decision rules

1. **Rank** by score. Within a tie (under 2 points), prefer higher R2, then fewer build days, then
   higher M2.
2. **First-sale rule.** Until the portfolio has 3 paid sales, the top slot needs R2 ≥ 3 (some warm
   access) **and** a build of 5 days or less. If nothing qualifies, take the highest-scoring item
   that builds in 5 days or less, and double its minimum launch exposure. This turns [IDEAS]'s
   manual override (formula library ahead of the ACX kit) into a rule.
3. **Capacity.** One product in creation at a time in the MVP, two in Phase 2. Each plan has at
   most 3 items.
4. **Portfolio balance.**
   - The first 3 products may share a cluster, which is good for ladder synergy and shared channels.
   - From product 4 on, no cluster or sales channel may hold more than 60% of active products.
   - Once there's a winner, 1 slot in 4 is for *explore* (a new cluster scoring ≥ 65). The rest
     are *exploit*: adjacent pockets or the next tier of a winner ([DV] §6, "keep digging").
   - No two products for the same pocket, except as tiers of one ladder.
5. **Format, picked by the buyer's job.**
   - *Look something up* → a library or cheat sheet plus a CSV or copy-paste index.
   - *Get through a process with a deadline* → a runbook, a checklist and a tracker spreadsheet.
   - *Fix a configuration* → presets or templates plus a short guide.
   - *Make a decision* → a decision tree.

   Use the shortest asset that gets the buyer to point B: 5–15 pages for a checklist, 20–45 for a
   playbook. Every product must contain something AI can't fake, such as tested code or the
   operator's own presets ([SYS] §5.6). Courses, subscriptions and "digital minds" come only after
   30+ sales of a lower tier ([PT] §3.2).
6. **Price ladder.** No pricing method was taught ([PT] §5), so this is our rule:

   | Tier | What | Price |
   |---|---|---|
   | 0 | Free sample (10–15% of the product), used as a value post | $0 |
   | 1 | Core MVP | B2C $19–39, B2B single user $29–49 |
   | 2 | Kit (templates, runbook, tracker) | $79–149 |
   | 3 | Team or partner licence | 2.5–3× the single price |
   | 4 | Course, updates subscription, digital mind | After 30+ tier-1/2 sales in the cluster |

   **Anchor:** 10–25% of the cheapest paid alternative in the evidence pack (a service, course or
   consultant hour). Then fit the price to the band of comparable products and round to $x9.
   - Never price below $15 net of fees.
   - A launch discount of up to 25% for 14 days needs G3.
   - Agents never give discounts on request (Project Vend, [SYS] §6).
7. **Pre-sell check.** Required when a product costs $99 or more or takes more than 5 days to
   build: 5 warm conversations, or one problem-only community post. We need at least 3 "that's me"
   answers ([S02a] §10.4).
8. **Sales channel.** Default to Whop. Gumroad is second. No Etsy for AI-assisted guides. No KDP
   for now ([SYS] §4).

**Output:** `products/plan/YYYY-Www.md` (human-readable) and `plan.json`. For each item:
- rank, slug, score, gate status and tie-break reasons
- the promise, the A/B map and the format with its deliverables
- price, ladder tier, build days, launch channels with R1/R2 notes
- "why it might fail"
- the evidence still missing

**Gate: G1 (enter a niche and start a product).** The default is to do nothing. The operator can
approve, reject, edit (change the promise or price), or send it back with `evidence` (one more S2
cycle).

---

## 5. MVP implementation plan

**Build order**

| When | What |
|---|---|
| **Nov 10–15** (execution break) | **Don't build the system.** Build product #1 by hand ([IDEAS] 5-day plan). Write `system/operator-profile.md`, including the warm-access counts. Spend 15 min confirming the paid evidence for N2 (see §6) |
| **Week of Nov 16** | Create the files: `system/scoring/weights-v1.json`; `scripts/score.py` (totals, gates, status, plan table; about 1 h); prompts in `system/prompts/{seed,pocket,evidence,score,plan}.md`; `research/niches/index.json` seeded with the 30 [IDEAS] ideas. Run S0–S4 once in an **interactive Claude Code session** for one seed and check the quality of the packs |
| **Week of Nov 23** | Turn the stages into **3 Claude Code routines** (below). First full weekly cycle |
| **After 4 cycles or the first launch result** | Review. A Telegram bot replaces `queue.md`, using the same item IDs and `decisions.jsonl` ([SYS] Phase 2) |
| **After 10 launches** | Refit the weights (§2.4) |

**Weekly cadence** (Thailand time; routines are capped per day on some plans, *[unverified]*, and
this schedule needs 3 runs a week)

| Day | Who | What |
|---|---|---|
| Mon 06:10 | Routine A, "research" | S0–S2: seeds, pockets, 8 evidence packs, `manual_checks` list |
| Mon–Tue | Operator, 20–30 min | Does the manual checks (Trends, Amazon, Facebook/Slack/Reddit browsing). Ticks them in `evidence.md`. Confirms R2 |
| Wed 06:10 | Routine B, "score and plan" | S3–S4: scores, promises, ranked plan, new queue entries |
| Wed–Thu | Operator, 15 min | G1 decisions in `queue.md` |
| Fri 06:10 | Routine C, "hand-off" | S5: creates product folders, logs rejects with reasons, updates `index.json` |

**Approval queue** (`system/approvals/queue.md`, until Telegram exists):

```markdown
## G1-2026-W48-01 · netsuite-saved-search-formulas · 79.2 · gates ✓ · rank 1/3
Promise: I help NetSuite admins … get a working formula for 100+ common reports in minutes.
Format: PDF + CSV index + flowchart · Price: $39 (tier 1) · Build: 3–4 days · R2: 4 (confirm)
Evidence: research/niches/netsuite-saved-search-formulas/evidence.md
Why it might fail: SuiteQL is replacing saved searches; free AI answers; small audience.
decision:
note:
```

The operator writes `approve`, `reject`, `edit` (with the change in `note:`) or `evidence`.
Routine C acts only on those exact words. A blank line or anything else means no action.

**Guardrails** ([SYS] §5.5):
- Each routine has a $5 cap and a maximum number of turns.
- A `system/PAUSED` file stops every routine.
- No posting or payment credentials anywhere in this pipeline.
- The scoring agent works from evidence packs only.
- Duplicates are checked against `index.json`.

**MVP is done when:** one weekly cycle produces at least 5 evidence packs, at least 3 scored passes,
a ranked plan and handed-off folders, without the operator shuffling files by hand, for $25 a week
or less and 90 minutes or less of operator time.

---

## 6. Validation: re-scoring the top ideas with v1

These are the top 5 by score in [IDEAS] §4, plus the two other products in its curated "Top 5
overall" table (N2 and N1). D1–D5, M2 (was F1), R1 (was F2), B1 (was F4), B3 (was F5) and B4 (was
F6) keep the [IDEAS] values. M1, M3, R2 and B2 are new and scored from the [IDEAS] evidence.

**The R2 values are our assumptions** from the owner's NetSuite consulting network. He has to
confirm them.

| Idea | D1 D2 D3 D4 D5 | M1 M2 M3 | R1 R2 | B1 B2 B3 B4 | Old | **v1** | Status |
|---|---|---|---|---|---|---|---|
| N5 Go-live CSV import kit | 4 5 4 4 4 | 3 5 4 | 3 3 | 5 5 4 5 | 84.6 | **79.8** | recommend (pre-sell check: $99) |
| A1 ACX Pass Kit | 4 4 5 5 5 | 4 3 4 | 4 **1** | 5 5 5 **4** | 85.6 | **79.6** | recommend, fails the first-sale rule (R2 1) |
| N2 Saved search formula library | 4 3 4 4 5 | **3** 4 4 | 4 **4** | 5 5 5 5 | 81.2 | **79.2** | recommend, **#1 in the plan** |
| N1 SOAP→REST / OAuth 2.0 kit | 3 5 4 4 4 | 3 5 4 | 3 4 | 5 5 3 5 | 80.0 | **78.0** | recommend, too big for now (7–10 days) |
| N11 EDI onboarding kit | 4 5 4 5 4 | 3 5 4 | **2 2** | 5 4 4 5 | 84.6 | 77.6 | **rejected: access gate** |
| J1 Spring Boot 3.5→4 playbook | 4 5 4 4 4 | 3 4 **2** | 4 2 | 5 5 4 5 | 83.0 | **76.2** | recommend, weak gap |
| J4 JVM-on-Kubernetes memory kit | 4 4 5 5 5 | **2** 4 3 | 3 2 | 4 5 5 5 | 83.4 | 74.6 | **needs_evidence: demand gate** (no paid solution shown) |

**What changed**

- **Warm access plus the first-sale rule now reproduce [IDEAS]'s manual pick (N2 first) by rule.**
  N5, A1 and N2 are tied (within 0.6 points). A1 fails the rule (R2 1, cold posts only). N5 fails it
  on build time (5–7 days). N2 qualifies (R2 4, 3–4 days).
- **The demand gate catches two things the old model missed.** J4 has search signal but no paid
  solution in the evidence, so it's parked. N2 passes only just (M1 3): the paid proof is indirect
  (consultants, official training, vendor SEO). **Before Nov 11, about 15 min:** find 1–2 Fiverr or
  Upwork gigs or consultant offers for saved-search formulas. If there are none, N2 goes to
  `needs_evidence`. Nothing else then meets the first-sale rule, so the fallback is A1 (3–4 days)
  with double exposure.
- **The access gate makes leaving N11 out a rule.** If the operator has 10+ wholesale clients who
  run EDI, R2 becomes 3 and N11 comes back at 79.2.
- **A1 loses 6 points:** R2 is 1, and B4 is 4 because ACX's "overall quality" call is outside our
  control, so we must never promise acceptance.
- **Scores bunch together** (74.6–79.8), so the gates and the tie rule do the real separating.
  Re-check this at the 10-launch refit.

**Proposed plan:** (1) N2 at $39 → (2) N5 at $99/$249, after the pre-sell check with partner
contacts → (3) N1 at $149/$399 before the 2027.1 deadline. One ladder, one cluster, shared channels.

---

## 7. Open questions

1. **Warm-access data:** what exactly goes in `operator-profile.md`? Counts per buyer role only, or
   also opt-in contact lists stored outside git? It's personal data under the GDPR.
2. **Episode 3** may show the course's distribution method (partner audiences, revenue shares). R1
   and R2 might need a "partner placement available" anchor, and pricing might need a revenue-share
   haircut.
3. **Keyword data:** DataForSEO pay-per-call or Google Ads Keyword Planner, and at what monthly cap
   (G5)?
4. **Claude Code routines:** what are the run caps on our plan, can a routine commit to this repo,
   and to which branch?
5. **Calibration before 10 launches:** should the operator also rank the 30 ideas by gut, so we can
   compare with v1 now?
6. **The B1 gate blocks the course's "zero expertise" niches.** Do we relax it later with a paid
   expert reviewer (G5)?
7. Do Whop receipts satisfy company-card buyers (VAT IDs, team licences)? This decides whether a high
   M2 actually turns into sales.
8. **Where the threshold sits:** is 65 right for `cheap_test` when building a product costs 3–7 days
   of operator time, not the course's "40 minutes"?
