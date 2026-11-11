# Ideas backlog

Ideas for the system, the research and the business. Not decided yet: each idea is discussed,
then accepted into `system/` requirements, parked, or dropped.

Status: 💡 new · 🔍 researching · ✅ accepted (moved into requirements) · 🅿️ parked · ❌ dropped

| # | Idea | Status | Notes |
|---|---|---|---|
| 1 | **Two research layers:** (a) **demand**: what people need and search for; (b) **bestsellers**: what currently sells best, then make new, better products based on those proven ideas | ✅ | See [below](#1-two-research-layers). Accepted into [`system/requirements.md`](../system/requirements.md) |
| 2 | **Build our own system instead of paying ~$2,000 for Monetize / Synthesize AI.** Use Claude (Ultra subscription) for what their tools do | ✅ | **Decided 11 Nov: don't buy Monetise ($1,995) now; build our own.** Re-decide after 6 weeks of building and outreach, only if the triggers in [the analysis](../research/monetise-vs-own-system.md#8-recommendation) §8 hold. In requirements as D-1 and the "build first" list. The course demo showed nothing that can't be rebuilt ([02b-develop](../course/sessions/02b-develop.md) §5) |
| 3 | **Find the best tools for market analysis.** Claude may not be the best at everything; compare Perplexity, others and paid data tools. Open to new subscriptions | 🔍 | Research sprint S3 (Claude vs Perplexity test), then phase 2 ([roadmap](../system/roadmap.md)) |
| 4 | **Study other systems and teachers, not only Iman's**, during research | 🔍 | Research sprint S1 → `research/other-systems.md` ([roadmap](../system/roadmap.md)) |
| 6 | **Three distribution channels**: partner creators, owned faceless channel, marketplaces. Compare cost per sale and operator time | ✅ | Into requirements R12. From [03a](../course/sessions/03a-vip.md) and [03b](../course/sessions/03b-distribute-deliver.md) |
| 7 | **"Ghost producer" model**: we build products for micro-creators who have an audience but no product, for a revenue share | 🔍 | The course's main method. Strong but needs operator time (calls, contracts). Research launch formats first |
| 8 | **Creators that already sell = bestseller dataset** for their niche (product, price, platform) | ✅ | Into R2c |
| 9 | **Pre-sale or waitlist** before building, as the cheapest proof people will pay | 💡 | Into R4b, operator gate |
| 10 | **Market-by-market research (country × language)**: analyse demand and bestsellers separately per country and language, finer than typical global tools, so we can sell a product in the specific markets where it fits | ✅ | Operator idea (11 Nov), backed by the course (Day 4 VIP: own language is "one of the biggest competitive advantages"; less advanced markets). Into requirements R1c. See [below](#10-market-by-market-research) |
| 5 | **Don't target the operator's own professions** (Java, NetSuite). Professionals there solve problems with AI and research and wouldn't buy a PDF | ✅ | Operator insight, see [`knowledge/operator/`](../knowledge/operator/). The course also says the market doesn't care about your passion ([choosing-products](../course/knowledge/choosing-products.md)) |

---

## 1. Two research layers

**Layer A: Demand ("what do people need?")**
- What problems people have, what they search for and ask about, how painful and urgent it is.
- Signals: search volume and trends, recurring questions in communities, complaints, reviews of
  existing solutions ("I wish it had…").
- Output: problems and "profitable pockets" with evidence of demand.

**Layer B: Bestsellers ("what already sells?")**
- What digital products currently sell best, on which platforms, at what price, in which format.
- Signals: bestseller and trending lists, sales and review counts, ranking over time, top creators.
- Then: **copy the idea, not the product.** Make a new product for the same proven demand that is
  better, more specific or for a narrower audience. Never copy content, branding or design.
- Output: proven product patterns (niche × format × price × positioning) with sales evidence.

**Combining them:** the best opportunities show up in both layers: real demand **and** proof that
people pay for this kind of product, plus a gap our product can fill (better, more specific,
faster).

Open points:
- Data sources for each layer (which platforms show sales or ranking data, and what may be
  automated) are a Phase 2 question.
- Where the line is between "inspired by" and "copying": legal and platform-rule check needed.

---

## 10. Market-by-market research

**Idea (operator, 11 Nov):** most tools look at "the market" globally, usually in English. We analyse
each **niche × country × language** separately and sell where a product fits best.

- The same problem can have strong demand and few products in one country/language and be saturated
  in another (e.g. a topic crowded in English but empty in Polish, German or Portuguese).
- Price levels, platforms, payment methods and buyer habits differ by country.
- AI makes localisation cheap: one validated product can be adapted to several markets.

What the research layers need to do per market:
- **Demand:** local search volume and trends, local communities and forums, questions in that language.
- **Bestsellers:** local marketplaces and creators, what sells and at what price in that currency.
- **Gap:** compare markets side by side: where is demand high and supply low?
- **Fit:** purchasing power, payment methods, platform availability (Whop, local alternatives), legal
  or tax limits, and whether we can check quality in that language.

Open questions for phase 2: which data sources give country- and language-level data (search tools,
marketplaces by country, creator databases with audience location), and at what cost.
