# Product ideas that fit the owner's own expertise (audio, Java, NetSuite)

> **Deprioritised (9 Nov).** The operator decided not to target his own professions (Java,
> NetSuite): professionals there solve their problems with AI and research and wouldn't buy a PDF.
> Kept as reference; the audio ideas (e.g. ACX kit, aimed at authors, not engineers) may still be
> relevant. See [knowledge/operator](../knowledge/operator/insights.md).


*Research report, 9 Nov 2026. This is our own research, not course material. Scores use the draft model in [`course/sessions/02a-vip-choosing-products.md` §10](../course/sessions/02a-vip-choosing-products.md).*

## Summary (10 lines)

1. All 30 ideas are in areas the owner can check himself. 27 pass the hard gates. Three fail on pain (D1 < 3) and are listed as rejected.
2. **The best score is the ACX Pass Kit for self-narrating authors (85.6).** Next come the NetSuite go-live CSV import kit and the NetSuite EDI onboarding kit (84.6 each), the JVM-on-Kubernetes memory kit (83.4) and the Spring Boot 3.5→4 upgrade playbook (83.0).
3. **NetSuite has the strongest economics.** Buyers spend company money and face hard deadlines: Oracle removes SOAP in 2028.2, and Poland's KSeF penalties start 1 Jan 2027. In our searches, nobody sells paid template or formula products for NetSuite on Gumroad, Payhip or Etsy. The competition is free vendor blogs (many look AI-written) and official training at $1,595–$5,000 per course.
4. **The weak point for NetSuite is distribution.** The communities are small: r/Netsuite has about 29k members, the NetSuite Professionals Slack said "5,000+" around 2019, and the largest regional user groups have 1–2k. These are B2B channels (LinkedIn, Slack, user groups), and Whop marketplace discovery will do almost nothing here.
5. **Audio has the biggest communities but mostly hobby (pleasure) pain.** The exceptions are tied to money or a pass/fail gate: ACX rejection, unpaid revisions, festival or distributor QC, and Atmos deliverables. Ambisonics is the owner's rarest skill, but the market is small and full of free academic tutorials (score 65.4).
6. **For Java, a paid info-product market is proven, but the generic part is crowded.** Javin Paul's Spring Boot interview book shows 813 sales at $19.90, but many sellers price at $1.99. Deadline products do better: Spring Boot 3.5 open-source support ended 30 Jun 2026, and Red Hat OpenJDK 8 enters extended support in Nov 2026.
7. **The owner's unique overlap is Java × NetSuite.** The SOAP→REST / OAuth 2.0 migration kit (80.0) has the highest price ceiling ($149–$399) and a hard Oracle deadline. It takes too long to build in one week, so it should be product #2 or #3.
8. **Recommended first product, Nov 11–15: the NetSuite saved search formula library** ($39, score 81.2). It's the fastest to build and test from his own consulting work. The pain shows up as an error every day. No paid competitor turned up. His existing NetSuite network makes a first sale most likely.
9. **Caveats:** reddit.com, gumroad.com, whop.com, udemy.com and etsy.com were blocked from direct fetching in this session. Every member count, price and sales figure comes from search-engine snippets or third-party trackers (GummySearch closed on 30 Nov 2025, so its numbers are stale). Google Trends was not checked. Treat counts as ±30%.
10. Before posting, check each community's self-promotion rules (unverified for r/Netsuite and the NetSuite Professionals Slack). Use "for NetSuite" wording, not Oracle branding. Build and test only in an account he is licensed to use for this, not a client's sandbox.

## Top 5 overall

| # | Product | Area | Score | Price | Why it's in the top 5 | Build time |
|---|---|---|---|---|---|---|
| 1 | **ACX Pass Kit**: presets, a noise-floor/RMS decision tree and a pre-submission QA sheet for self-narrating authors | Audio | **85.6** | $39 ($59 with all DAW presets) | Clear pass/fail outcome (ACX accepts or rejects). The same complaint repeats for years on the Audacity forum. Courses cost up to $497 and a narrator costs $100–500 per finished hour, so $39 is an easy yes. He can check every claim himself with ACX Check and his own ears. | 3–4 days |
| 2 | **Saved search formula library**: 100+ tested formulas plus an "Invalid Expression" decoder | NetSuite | **81.2** | $39 (launch $29) | Admins and finance users hit it every day. People keep asking the same CASE WHEN questions. No paid product found, only free blogs. Shortest build. Warm network. | 3–4 days |
| 3 | **Go-live CSV import kit**: import-order map, templates, validation checklist, error decoder | NetSuite | **84.6** | $99 single / $249 team | Hard go-live deadline. Mistakes cost money. Buyers pay with company cards. Can be sold to small implementation partners too. | 5–7 days |
| 4 | **JVM-on-Kubernetes memory kit**: OOMKilled decision tree, sizing calculator, flags cheat sheet, Grafana panel | Java | **83.4** | $29 | Production restarts cause pain several times a day. The result can be measured (exit 137 stops). Small and quick to build. Risk: lots of free blog posts, so it has to win on speed and certainty. | 2–3 days |
| 5 | **SOAP→REST / OAuth 2.0 migration kit for NetSuite integrations**: inventory searches, Java and Node OAuth 2.0 reference clients, cutover runbook | NetSuite × Java | **80.0** | $149 single / $399 team | Oracle's own timeline: new builds on REST from 2026.1, no new SOAP or TBA integrations from 2027.1, SOAP removed in 2028.2. Only someone who knows both NetSuite and Java can verify this kit. Highest price ceiling. | 7–10 days (not for this break) |

**Left out on purpose:** the **EDI trading-partner kit (84.6)** has a top score but reach of 2: its buyers (ops and IT at distributors) are hard to find without paid ads. Keep it as a later B2B upsell. The **Spring Boot 3.5→4 playbook (83.0)** competes with many free migration guides and free AI "skills" files. It's a good fourth or fifth product while the Boot 4.0 support window is in the news.

### Recommended first product (Nov 11–15): the saved search formula library

**Promise:** *"I help NetSuite admins and finance power users whose saved-search formulas keep throwing 'Invalid Expression' while report requests pile up get a working, copy-paste formula for 100+ common reports in minutes, not hours."*

Why it comes first, ahead of the ACX kit that scores higher:
- **Chance of a first sale.** As a consultant, the owner has warm contacts: clients, colleagues and LinkedIn. The ACX kit would rely only on cold posts in communities where he has no history. The research doc notes that the best-known "AI business" success sold mostly to an audience its owner already had.
- **Speed and verification.** Most formulas already exist in his past work. Each one is checked by running it: it either returns the right column or it doesn't. AI can draft the explanations; he tests every formula.
- **Platform risk is low.** Whop is the merchant of record. Etsy is skipped, because a formula library could count as a "functional guide" under Etsy's 22 Oct 2026 AI rules ([ppc.land](https://ppc.land/etsy-forces-sellers-to-show-one-unaltered-photo-in-every-listing/), [cryptobriefing](https://cryptobriefing.com/etsy-bans-ai-generated-recipes-patterns/), secondary sources).
- **It starts a product ladder:** formula library ($39) → SuiteQL pack ($49) → go-live CSV kit ($99–249) → SOAP→REST kit ($149–399).

**5-day plan**
- **Nov 11:** Pull the 30 most-asked formula questions from the NetSuite Professionals archive and the Oracle community (links in §1.2). Add his own snippets and fix the table of contents: by record type and by report (AR aging, days-to-ship, margin, last-activity, consolidated text, etc.).
- **Nov 12–13:** Write and **test each formula in a NetSuite account he may legally use for this.** Do not use a client's sandbox without permission. Check whether he has access to a partner or SuiteCloud developer account (**unverified**). Record the field type (Text, Numeric, Date, Currency), the summary type and known gotchas: smart quotes, CASE without END, aggregates inside CASE.
- **Nov 14:** Format the deliverables: a PDF, a copy-paste text/CSV index and a one-page "Invalid Expression" flowchart. Create the Whop product (hidden), the listing copy and a free 10-formula sample PDF as a lead magnet.
- **Nov 15:** Publish. Post the free sample on LinkedIn. Post it in r/Netsuite and the NetSuite Professionals Slack **only if their rules allow** (check first). DM 10–20 warm contacts.
- **Kill or iterate:** if there's no sale after about 3 weeks of honest distribution, revisit the scoring (research doc, exec summary #10).

**Why it might fail:**
- Oracle is pushing SuiteAnalytics Workbook and SuiteQL, so saved searches may slowly lose relevance.
- Free AI answers (the archive's own AI bot, ChatGPT) may be "good enough" for many buyers.
- The audience is small.

---

## 0. Method and scoring

**Scoring model (from 02a §10):**
- Desirability (60%): D1 Pain 20, D2 Worsening 12, D3 Transformation 12, D4 Specificity 10, D5 Speed 6.
- Feasibility (40%): F1 Ability to pay 12, F2 Reach 10, F3 Competition/proof 6, F4 Operator verifiability 7, F5 Effort/format fit 3, F6 Policy/claim risk 2.
- Total = Σ(score × weight) / 5, which gives 0–100.
- **Hard gates:** D1 < 3, D4 < 3, F4 < 3 or F6 = 1 means reject. A score of 75 or more means "recommend"; 60–74 means "needs evidence".
- Per-criterion scores are listed as `D1 D2 D3 D4 D5 | F1 F2 F3 F4 F5 F6`.

**How the evidence was gathered:**
- Web search only. Direct fetches of reddit.com, gumroad.com, whop.com, udemy.com, etsy.com, gearspace.com and kvraudio.com were blocked by this session's network policy. To check them directly, those hosts have to be allowed in the session's network settings.
- Prices, sales counts and member counts therefore come from search-engine snippets of those pages, or from aggregators (GummySearch, The Hive Index, painonsocial, comidoc, ctgoodjobs).
- GummySearch closed on 30 Nov 2025, so its counts are historical.
- **[unverified]** marks claims backed by only one weak source, or sources that disagree.
- I scored F4 (verifiability) from the skills listed in the brief. Where an idea needs a sub-skill the brief doesn't mention (live sound, film post, Kubernetes), I lowered F4 and flagged it.

**B2B versus B2C:**
- **NetSuite buyers** (admins, controllers, project leads) pay with company money and accept $49–$399. They don't browse Whop or Etsy. Reach comes from LinkedIn, the NetSuite Professionals Slack, r/Netsuite, regional user groups and SEO. They may want a VAT invoice and a "team license". Check that Whop receipts satisfy them **[unverified]**.
- **Audio buyers** are mostly B2C: lower prices, bigger communities, strict self-promotion rules.
- **Java** sits in between: individual developers pay $20–50, and team or employer-paid licenses work for upgrade or migration kits.

---

## 1. NetSuite (ERP: SuiteScript, SuiteApps, EDI, e-invoicing, implementations, audits)

### 1.1 Where buyers gather

| Community | Size | Notes |
|---|---|---|
| r/Netsuite | ~29k, +27.9%/yr | [GummySearch](https://gummysearch.com/r/Netsuite) (stale tracker). Self-promotion rules **unverified** |
| r/NetSuite_Users | ~2k | [GummySearch](https://gummysearch.com/r/NetSuite_Users) |
| NetSuite Professionals Slack + Q&A site | "over 5,000 members" (text from ~2019, surely more now **[unverified]**). Active in 2025–26 | [about](https://netsuiteprofessionals.com/about-us/), [archive activity](https://archive.netsuiteprofessionals.com/t/30363226/hello-fam-glad-to-join-the-netsuite-community-i-m-sherman-lu) |
| Oracle NetSuite Support Community + regional user groups | NY Metro 1,800+, Rocky Mountain 1,500+, Boston 1,115, Southeast 300 | [groups directory](https://community.oracle.com/netsuite/groups). Vendor promotion probably not allowed |
| Customer base (the total market) | 40,000+ (some sources say 43,000+) customers | [Cazoomi](https://www.cazoomi.com/blog/top-15-netsuite-statistics-you-should-know-in-2025-and-beyond/), [AppsRunTheWorld](https://www.appsruntheworld.com/oracle-netsuite-expands-cloud-erp-with-ai-applications-tools) **[third-party]** |
| Job market (ability to pay) | US NetSuite admin pay roughly $80k–$130k | [ZipRecruiter](https://www.ziprecruiter.com/Jobs/Netsuite-Admin), [KORE1](https://www.kore1.com/netsuite-administrator-salary-guide/) |

### 1.2 Recurring pain (evidence)

- **Saved search formulas (CASE WHEN, "Invalid Expression").** The same question keeps coming back: [archive 1](https://archive.netsuiteprofessionals.com/t/94763/hi-folks-i-m-having-trouble-getting-a-case-when-statement-wo), [archive 2](https://archive.netsuiteprofessionals.com/t/16660127/can-someone-help-with-a-case-when-formula-i-m-trying-to-crea), [archive 3](https://archive.netsuiteprofessionals.com/t/97899/ok-all-you-saved-search-mavens-out-there-i-m-trying-to-do-a-), [Oracle community](https://community.oracle.com/netsuite/english/discussion/4492247/nsc-saved-search-formula-resolve-error-invalid-expression-case-when-with-sum-formula), [NSP Q&A](https://netsuiteprofessionals.com/blog/question/saved-search-invalid-expression-error/). Vendors write SEO posts about it ([Anchor Group](https://anchorgroup.tech/why-your-netsuite-saved-search-case-when-is-broken), [Versich](https://versich.com/blog/fixing-your-netsuite-saved-search-case-when-errors/)), which shows commercial interest. Many threads stay unresolved.
- **Advanced PDF/HTML (FreeMarker) templates:**
  - Threads: [archive](https://archive.netsuiteprofessionals.com/t/27080602/in-netsuite-i-m-trying-to-customize-the-standard-purchase-pd), [archive](https://archive.netsuiteprofessionals.com/t/2577248/anyone-have-issues-with-advanced-pdf-html-freemarker-templat), [Oracle community](https://community.oracle.com/netsuite/english/discussion/4487136/new-to-netsuite-advanced-pdf-html-templates/p1).
  - People already pay for it: [Fiverr gig](https://fiverr.com/wajih_123/do-netsuite-advanced-pdf-templates).
- **SuiteScript governance (SSS_USAGE_LIMIT_EXCEEDED):** [archive](https://archive.netsuiteprofessionals.com/t/16016936/any-suggestions-for-dealing-with-governance-in-a-map-reduce-), [archive](https://archive.netsuiteprofessionals.com/t/224015/how-to-overcome-sss-script-usage-limit-exceeded-error-in-sui), [archive](https://archive.netsuiteprofessionals.com/t/27011720/how-to-resolve-script-execution-usage-limit-exceeded), [Oracle doc](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4480364878.html).
- **CSV import and data migration:**
  - Recurring errors: [archive](https://archive.netsuiteprofessionals.com/t/33137430/i-received-the-error-message-an-unexpected-error-has-occurre), [NSP blog](https://netsuiteprofessionals.com/blog/administration/7-common-netsuite-csv-import-errors-and-how-to-solve-them/), [Salto](https://salto.io/blog-posts/netsuite-csv-import-errors).
  - Imports show only the first error, so they need repeated test passes ([Oracle FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3924743.html), via a search summary).
  - I found no go-live migration template for sale.
- **Implementations and post-go-live:**
  - "Spend an afternoon in r/Netsuite" and the pattern is a bad go-live blamed on the partner ([Houseblend](https://www.houseblend.io/blog/will-your-netsuite-implementation-partner-help-or-hurt-you), vendor).
  - Partner hand-offs fail ([KORE1](https://www.kore1.com/netsuite-rescue-staffing/)). Problems often appear after go-live ([Concentrus](https://concentrus.com/?p=4485)).
  - Typical project is 4–9 months ([Epiq](https://epiqinfo.com/?p=997224)).
- **SOAP retirement, a hard deadline:**
  - Oracle: REST with OAuth 2.0 for new builds from 2026.1. No new SOAP integrations from 2027.1. SOAP removed in 2028.2 ([Oracle SOAP Removal FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_2104046421.html)).
  - No new TBA integrations from 2027.1 ([Workato](https://www.workato.com/product-hub/netsuite-integrations-integration-strategy-workato/)).
  - Other sources give different dates ([RSM](https://technologyblog.rsmus.com/technologies/netsuite/netsuite-2026-1-critical-changes-clients-must-address-now/) says migrate by 2029.1, [KingswaySoft](https://www.kingswaysoft.com/resources/industry-trends/netsuite-retires-soap-api)), so treat Oracle's FAQ as the reference.
- **Renewal price rises:**
  - Reddit users quoted saying "16% increase … we can barely afford it" and "usually 5–7% … this year 11%" ([Prospeo aggregate](https://prospeo.io/s/oracle-netsuite-pricing-reviews-pros-and-cons), secondhand).
  - [Oracle community thread](https://community.oracle.com/netsuite/english/discussion/4217048/new-renewal-prices).
  - Consultancies sell negotiation help ([OLE](https://oraclelicensingexperts.com/blog/netsuite-renewal-strategy/), [Redress](https://redresscompliance.com/netsuite-pricing-negotiation)).
- **EU e-invoicing mandates:**
  - Poland KSeF: mandatory for most firms from 1 Apr 2026, smallest firms from 1 Jan 2027 ([MF official](https://ksef.podatki.gov.pl/etapy-wdrozenia-ksef)). Penalties from 1 Jan 2027 according to [PARP](https://uslugirozwojowe.parp.gov.pl/wyszukiwarka/uslugi/drukuj-pdf?id=3270382); sources disagree, one says Aug 2026.
  - Belgium B2B from 1 Jan 2026 ([Lexgo](https://www.lexgo.be/en/news-and-articles/14132-e-invoicing-mandatory-in-belgium-from-1-january-2026)).
  - France: everyone must receive from 1 Sep 2026; smaller firms must issue from 1 Sep 2027 ([Ebner Stolz](https://www.ebnerstolz.de/en/what-we-offer/services/tax-advice/value-added-tax/e-invoicing-and-e-reporting-france-110656.html)).
  - Germany: issuing required above €800k turnover from 1 Jan 2027 ([VATit](https://businessbonus.vatit.com/es/e-invoicing-guide/germany/)).
  - NetSuite routes for KSeF: APLP or the Electronic Invoicing Builder ([Houseblend KSeF guide](https://www.houseblend.io/articles/fr/poland-ksef-2026-netsuite-setup-guide)).
- **EDI:** problems include partner rules tracked in spreadsheets, chargebacks and slow onboarding ([Cleo](https://www.cleo.com/lp/netsuite-edi-integration/), [Broken Rubik](https://www.brokenrubik.com/blog/netsuite-edi-integration-guide), [Houseblend control matrix, Oct 2026](https://www.houseblend.io/articles/netsuite-edi-control-matrix-reconciliation)). All vendor sources.

### 1.3 Existing paid products and prices

| Product | Price | Proof of demand | Source |
|---|---|---|---|
| Official NetSuite instructor-led training | $1,595–$1,600 for 2-day finance/controller courses; "$2,000–5,000 per course" | Price anchor showing buyers have budget | [Financial Mgmt](https://www.netsuite.co.uk/portal/uk/services/training/finance-fundamentals.shtml), [Controller](https://www.netsuite.com.au/portal/au/services/training/suite-training/description-controller.shtml), [community](https://community.oracle.com/netsuite/english/discussion/4248935/preparing-for-suitescript-course) |
| Udemy "NetSuite ERP: Ultimate … 2026" | Udemy pricing | Bestseller, 4.7 from 261 ratings, 1,302 students | [ctgoodjobs mirror](https://www2.ctgoodjobs.hk/Learning/1354974708/udemy/netsuite-erp-the-ultimate-complete-erp-training-course-2026) |
| Udemy "NetSuite Functional Ultimate Guide" | Udemy pricing | 3,315 ratings (last updated 2022) | [Udemy](https://www.udemy.com/course/netsuite-ultimate-functional-guide/) |
| Udemy SuiteScript courses | ~$19.99 | Weak: 47 students / 3.89; 95 students / 3.44 | [comidoc 1](https://comidoc.com/udemy/suite-script-with-ajax-online-form-by-using-htmltemplate), [comidoc 2](https://comidoc.com/udemy/learn-oracle-netsuite-client-script-20-k) |
| SuiteFoundation exam prep (Udemy) | Udemy pricing | 4.7 from 41 ratings | [ctgoodjobs](https://www2.ctgoodjobs.hk/Learning/1500644498/udemy/netsuite-suitefoundation-certification-prep-course) |
| Gumroad "Learn SuiteQL" ebook; "NetSuite ERP Career Guide" | SuiteQL price unknown; career guide $0+ with 3 ratings | Weak | [SuiteQL](https://saisunkara.gumroad.com/l/suiteql), [career](https://saisunkara.gumroad.com/l/netsuite) |
| Art of Service NetSuite "courses" | $198–$199 | Unknown (looks generic) | [example](https://store.theartofservice.com/mastering-netsuite-implementation-and-optimization-strategies) |
| FloQast month-end close checklist for NetSuite | Free (lead magnet) | Competition for the close idea | [FloQast](https://floqast.com/templates/month-end-close-checklist-oracle-netsuite) |
| Saved search, PDF template or CSV import products on Gumroad/Payhip/Etsy | **None found** | Gap, or no demand. Test cheaply | search, 9 Nov 2026 |

### 1.4 NetSuite ideas (12)

**N1. SOAP→REST / OAuth 2.0 migration kit (Java and Node)**
- Buyer: NetSuite admins or developers and integration owners at companies with SuiteTalk SOAP or TBA integrations; also small ISVs.
- Problem (worsening): new SOAP and TBA builds are blocked from 2027.1 and existing SOAP stops in 2028.2. Every month of delay compresses the project.
- Promise: *I help NetSuite integration owners whose SOAP/TBA integrations can't be built new after 2027.1 and stop working in 2028.2 get every integration inventoried and a tested OAuth 2.0 REST migration plan in 5 working days.*
- Format: PDF runbook, inventory saved searches and SuiteQL (integration records, login audit), an Excel tracker, Java and Node OAuth 2.0 client-credentials reference clients, cutover checklist.
- Price: $149 single / $399 team.
- Where: NetSuite Professionals Slack, r/Netsuite, LinkedIn, regional user groups.
- Competition: free vendor playbooks ([Truto](https://truto.one/blog/a-practical-netsuite-migration-guide-moving-off-soap-before-2028/), [GURUS](https://gurussolutions.com/blog/netsuite-soap-to-rest-migration)); iPaaS vendors migrating for their own customers ([Celigo](https://docs.celigo.com/hc/en-us/articles/54916543775643), [TrueCommerce](https://help.truecommerce.com/en/articles/12314782-netsuite-migration-from-soap-to-rest)). No paid kit found.
- Score: `3 5 4 4 4 | 5 3 4 5 3 5` → **80.0**. Pain today is moderate (D1 3) but rising, and the code needs sandbox testing (F5 3).

**N2. Saved search formula library + "Invalid Expression" decoder** (recommended first)
- Buyer: NetSuite admins, accountants and ops power users.
- Problem (worsening): report requests pile up every week, every failed formula costs an hour, and month-end makes it worse.
- Promise: see the recommendation above.
- Format: 40–60 page PDF, copy-paste CSV index, one-page flowchart.
- Price: $39.
- Where: r/Netsuite (~29k), NSP Slack (5k+), LinkedIn.
- Competition: free blogs only ([Nanonets](https://nanonets.com/blog/netsuite-saved-searches), [GURUS gated guide](https://gurussolutions.com/netsuite-saved-searches), [Oracle examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N691341.html)).
- Score: `4 3 4 4 5 | 4 4 4 5 5 5` → **81.2**.

**N3. SuiteQL query pack (75 finance and ops queries + join map)**
- Buyer: admins and analysts moving from saved searches to SuiteQL, ODBC or REST.
- Problem: joins return wrong totals, and the schema is poorly documented.
- Promise: *I help NetSuite analysts moving to SuiteQL whose joins return wrong totals get 75 tested queries and a table-join map in one afternoon.*
- Format: PDF + .sql files. Price: $49. Where: as N2.
- Competition: [Gumroad SuiteQL ebook](https://saisunkara.gumroad.com/l/suiteql), Tim Dietrich's free SuiteQL Query Tool, [Houseblend free guide](https://houseblend.io/articles/fr/netsuite-suiteql-custom-fields-joins).
- Score: `3 3 4 4 5 | 4 4 3 5 4 5` → **75.4**.

**N4. Advanced PDF/HTML template pack (invoice, statement, PO, packing slip, pick ticket; multi-currency and multi-language; FreeMarker snippets)**
- Buyer: admins told to "make the invoice look like our old one before month-end".
- Promise: *I help NetSuite admins whose invoice and packing-slip layouts embarrass them in front of customers get 8 polished, tested Advanced PDF templates live in one day.*
- Format: .xml/.ftl templates + install PDF. Price: $59–79.
- Where: as N2.
- Competition: Fiverr services; free how-tos ([RSM](https://technologyblog.rsmus.com/netsuite/freemarker-logic-and-advanced-pdfhtml-templates-with-netsuite), [Folio3](https://netsuite.folio3.com/blog/getting-started-with-netsuite-pdf-templates-a-beginners-guide)). No template packs found.
- Score: `3 3 5 4 5 | 4 4 4 5 4 5` → **79.0**. Very visible before/after result (D3 5). Pain is weekly, not daily.

**N5. Go-live data migration CSV import kit**
- Buyer: in-house project leads and admins less than 60 days from go-live; small implementation partners (sell them a partner license).
- Problem (worsening): test imports fail on "invalid reference key", and the go-live date doesn't move.
- Promise: *I help NetSuite project leads less than 60 days from go-live whose test imports keep failing get a clean, correctly ordered data migration run in two weekends.*
- Format: import-order dependency map, 15 record-type CSV templates, pre-import validation checklist (Excel), error decoder, cutover runbook.
- Price: $99 single / $249 team / partner license by quote.
- Where: NSP Slack, r/Netsuite, LinkedIn, partner networks.
- Competition: free blogs ([NSP](https://netsuiteprofessionals.com/blog/administration/7-common-netsuite-csv-import-errors-and-how-to-solve-them/), [Salto](https://salto.io/blog-posts/netsuite-csv-import-mistakes), [Cleverence](https://www.cleverence.com/articles/oracle-documentation/csv-imports-overview-netsuite-70493812/)), [NetGain data-cleaning checklist](https://support.netgain.tech/article/436485/netasset---data-cleaning-checklist-for-csv-uploads). No kit for sale.
- Score: `4 5 4 4 4 | 5 3 4 5 4 5` → **84.6**.

**N6. NetSuite renewal negotiation playbook (for CFOs and controllers)**
- Problem (worsening): quotes rise 5–16% and the 60–90-day notice window is closing.
- Promise: *I help NetSuite customers' CFOs whose renewal quote just jumped by double digits get a documented negotiation plan and asks in 7 days.*
- Format: PDF + timeline template + email scripts. Price: $149.
- Where: LinkedIn and CFO communities (hard to reach, F2 2).
- Competition: free white papers from consultancies ([OLE](https://oraclelicensingexperts.com/blog/netsuite-negotiation-tactics/), [Costbench](https://costbench.com/software/erp/netsuite/negotiation/)).
- Score: `4 5 4 5 4 | 5 2 3 3 4 3` → **79.8**. F4 is only 3 because current Oracle discount data is outside his day job. F6 is 3 because savings claims are risky: never promise a percentage.

**N7. SuiteScript governance and performance cookbook (Map/Reduce patterns, yield, batching, governance budgeting, plus a code library)**
- Buyer: SuiteScript developers whose scheduled scripts die as data grows.
- Promise: *I help SuiteScript developers whose scripts die with SSS_USAGE_LIMIT_EXCEEDED as volumes grow get production-safe Map/Reduce patterns in a weekend.*
- Format: PDF + repo zip. Price: $59.
- Where: NSP Slack, r/Netsuite.
- Competition: weak Udemy courses (3.4–3.9 ratings), Oracle docs, Houseblend blogs.
- Score: `4 3 4 4 4 | 4 4 4 5 4 5` → **79.4**.

**N8. Java developer → NetSuite developer career switch guide** (rejected)
- Score: `2 2 4 4 3 | 3 3 3 5 4 4` → **61.8**, fails the gate on D1.
- It's a want (career upside), not a pain, and it would need income claims (F6 risk). Background: [Houseblend career guide](https://www.houseblend.io/articles/netsuite-career-paths-guide), [Oracle community](https://community.oracle.com/Netsuite/english/discussion/4488231/what-kind-of-skills-are-needed-to-be-a-netsuite-developer).

**N9. EU e-invoicing readiness kit for NetSuite (PL KSeF, BE Peppol, FR, DE)**
- Buyer: finance and IT leads at NetSuite companies with EU entities.
- Problem (worsening): KSeF penalties from 1 Jan 2027, French and German issuing deadlines 2026–2028.
- Promise: *I help finance leads at NetSuite companies with Polish, Belgian, French or German entities facing 2027 e-invoicing penalties get a gap check and configuration checklist in one week.*
- Format: PDF + per-country checklist + test-case sheet. Price: $149.
- Where: LinkedIn, Polish finance groups, partners (F2 2).
- Competition: free partner guides ([Houseblend](https://www.houseblend.io/articles/fr/poland-ksef-2026-netsuite-setup-guide)), localisation SuiteApps.
- Score: `4 5 4 4 4 | 5 2 3 4 3 3` → **78.6**. The rules change often, so it needs maintenance. It's tax-adjacent, so F6 is 3. The owner is in Poland and does e-invoicing work, which is a real edge for the Polish part.

**N10. Month-end close pack for NetSuite controllers**
- Promise: *I help NetSuite controllers whose close slips past day 10 get a 30-step checklist with 15 reconciling saved searches in one close cycle.*
- Price: $49.
- Competition: free FloQast checklist; $198 Art of Service course.
- Score: `4 4 4 4 4 | 4 3 2 4 5 5` → **76.6**.

**N11. EDI trading-partner onboarding kit (850/855/856/810/997)**
- Buyer: ops and IT at NetSuite wholesalers onboarding a big-box retailer.
- Problem (worsening): chargebacks start with the first shipments.
- Promise: *I help NetSuite wholesalers onboarding a major retailer whose first chargebacks are landing get a partner mapping spec, test plan and chargeback-prevention checklist in 2 weeks.*
- Format: Excel mapping spec + PDF runbook. Price: $149–199.
- Where: LinkedIn, EDI-provider communities (F2 2).
- Competition: free vendor content (SPS, Cleo, Orderful). Managed EDI costs $200–1,500/month ([Broken Rubik](https://www.brokenrubik.com/blog/netsuite-edi-integration-guide)), which makes $199 cheap.
- Score: `4 5 4 5 4 | 5 2 4 5 4 5` → **84.6**.

**N12. "Inherited NetSuite account" health check (for new or accidental admins)**
- Promise: *I help newly hired NetSuite admins who inherited an undocumented account that breaks every week get a full health audit and prioritised fix list in 3 days.*
- Format: audit checklist (Excel) + saved searches (unused scripts, roles, workflows). Price: $49–79.
- Where: as N2.
- Competition: partner "health check" services (paid, $$$).
- Score: `4 3 4 4 4 | 4 4 3 5 5 5` → **78.8**.

---

## 2. Audio (mixing, recording, spatial/Ambisonics)

### 2.1 Where buyers gather

| Community | Size | Source |
|---|---|---|
| r/WeAreTheMusicMakers | ~3.8M (another snapshot says 1.7M) | [GummySearch](https://gummysearch.com/r/WeAreTheMusicMakers) |
| r/audioengineering | ~648–654k | [GummySearch](https://gummysearch.com/r/audioengineering), [Hive Index](https://thehiveindex.com/communities/r-audioengineering/) |
| r/audiobooks (mostly listeners) | ~232k | [painonsocial](https://painonsocial.com/subreddits/audio-book-narrators) |
| r/podcasting | ~163–194k | [GummySearch](https://gummysearch.com/r/podcasting) |
| r/mixingmastering | ~100–120k | [GummySearch](https://gummysearch.com/r/mixingmastering), [painonsocial](https://painonsocial.com/subreddits/mixing-engineers) |
| r/homerecording | ~100k **[single source]** | [painonsocial](https://painonsocial.com/subreddits/recording-engineers) |
| r/VoiceActing | ~41–67k (sources disagree) | [painonsocial](https://painonsocial.com/subreddits/narrators) |
| Gearspace | 400k+ members, 1.6M monthly visitors (figures from ~2021–22) | [Wikipedia](https://en.wikipedia.org/wiki/Gearspace), [Mix](https://www.mixonline.com/the-wire/gearspace-celebrates-20-years-as-the-worlds-biggest-pro-audio-forum) |
| Audacity forum: ACX threads | Many threads over years | see §2.2 |
| Whop music communities | e.g. SoniX Academy, free, 1,488 members | [third-party mirror](https://whopreviews-six.vercel.app/communities/kxvi-sonix-academy) |
| KVR (Ambisonics/IEM threads) | Size not found | [KVR thread](https://www.kvraudio.com/forum/viewtopic.php?p=8187067) |

### 2.2 Recurring pain (evidence)

- **ACX rejections (noise floor, RMS, peak):**
  - Fixing RMS and peak pushes the noise floor over the limit ([Audacity forum](https://forum.audacityteam.org/t/fixing-peak-and-rms-levels-makes-noise-floor-fail-acx-check/62493)).
  - Files pass in Audacity but fail at ACX ([forum](https://forum.audacityteam.org/t/noise-floor-passes-in-audacity-fails-in-acx/94865)).
  - "ACX say my RMS is too low" ([forum](https://forum.audacityteam.org/t/acx-say-my-rms-is-too-low/52123)).
  - Rejected for "overall quality" even after meeting the specs ([forum](https://forum.audacityteam.org/t/clips-meets-acx-standard-but-i-got-rejected-because-60db-noise-reduction/52502)).
  - Spec as quoted on the forum: RMS −23 to −18 dB, peak ≤ −3 dB, noise floor ≤ −60 dB ([forum](https://forum.audacityteam.org/t/problems-editing-audio-book-to-pass-acx/50493)). **Re-check against ACX's official page.**
  - Paid checker tools exist ([NarrationBox](https://narrationbox.com/tools/acx-compliance-checker), [Timbrica](https://timbrica.com/en/audiobook-checker)).
- **Freelance mixing business (revisions, pricing, contracts):** many free guides exist ([Violet Recording](https://violetrecording.com/how-to-handle-mix-revisions/), [Tape Op](https://tapeop.com/tutorials/73/intro-contracts)). One "studio client system" product is sold on [SoundBetter](https://my.soundbetter.com/info-tripledstudio/products/435-studio-client-system).
- **Podcast audio:**
  - In an informal poll, 54% of 305 respondents said bad audio is their main reason for abandoning a show ([podcast episode](https://metacast.app/podcast/be-a-better-podcaster-with-jamie-and-jaayne/ju0ESS8D/why-audio-quality-is-more-important-than-you-think/NI04JWPb)). Weak evidence.
  - Guests are the "wild card" ([East Coast Studio](https://eastcoaststudio.com/podcast/keep-every-listener-know-these-5-reasons-people-stop-listening-to-podcasts/)).
- **Atmos and spatial audio:**
  - Apple pays up to 10% more royalties for Spatial Audio tracks ([MacRumors](https://www.macrumors.com/2023/12/11/apple-music-to-incentivize-spatial-audio/)). Indie labels object ([MacRumors](https://www.macrumors.com/2024/02/02/apple-music-spatial-audio-royalties-big-companies/)).
  - "No upmixing" delivery rule per [Dynamoi](https://dynamoi.com/learn/apple-music-promotion/apple-music-spatial-audio-royalty-bonus) **[unverified, SEO site]**.
  - Atmos mixing estimated at ~$1,000 extra per song (FT-sourced, via MacRumors).
- **Loudness:** Spotify's official −14 LUFS / true-peak guidance is free and clear ([Spotify](https://support.spotify.com/artists/article/loudness-normalization/)), so selling it adds little.
- **Ambisonics:** good free tutorials exist ([IEM series](https://www.soundingfuture.com/en/hands-on/immersive-audio-production-iem-plugin-suite), [ICST](https://ambisonics.ch/page/2/)), plus university short courses ([Greenwich](https://www.gre.ac.uk/research/activity/las/spatial-audio-fundamentals)).

### 2.3 Existing paid products and prices

| Product | Price | Proof | Source |
|---|---|---|---|
| Gumroad vocal chains and mix templates | $4.99–$99 | Many pages show 0–1 sales: a saturated, low-trust market | [example $27](https://worksource1.gumroad.com/l/aucvk), [bundle](https://mixedbyyeldo.gumroad.com/l/ultimatevcmby) (via search snippets) |
| Podcast voice preset pack (Gumroad) | $95 | Unknown | [ryanfreeman](https://ryanfreeman.gumroad.com/l/LRmpy) |
| Music Radio Creative podcast presets | £13.95–£43.50 | Called "best selling" by the seller | [MRC](https://musicradiocreative.com/products/audacity-presets-for-podcasters) |
| Kindlepreneur "Audiobooks Made Easy" | $497 (page from 2021) | Price anchor for authors | [Kindlepreneur](https://kindlepreneur.com/courses/audiobooks-made-easy/) |
| Professional narrator rates | $100–$500 per finished hour | The alternative an author pays instead | [Chapter blog](https://blog.chapter.pub/how-to-record-your-own-audiobook/) **[blog figure]** |
| Dolby Atmos in Logic PDF | $10, 135 pages (2022) | Shows people pay for it; dated | [dingdingmusic](https://www.dingdingmusic.com/-titles-/dolby-atmos-3.html) |
| Atmos courses | $19.99 (Udemy) to £400 (GSA) to $1,495 (Audiograph) to $4,500 (1:1) | Wide price ladder | [Udemy](https://comidoc.com/udemy/learn-dolby-atmos-mixing-in-studio-one), [GSA](https://futureskills.gsa.ac.uk/dolbyatmos), [Audiograph](https://www.audiographintl.com/product-page/mixing-in-dolby-atmos-music-post-production) |
| Church X32 course and presets (Drew Brashler) | Price not shown | Niche creator business exists | [drewbrashler.com](https://drewbrashler.com/), [course](https://course.drewbrashler.com) |
| MixCoach membership | $295/yr | Membership benchmark | [MixCoach](https://www.mixcoach.com/mixcoach-member-pricing-spring-2024) |

### 2.4 Audio ideas (10)

**A1. ACX Pass Kit for self-narrating authors** (top overall score)
- Buyer: indie authors narrating their own audiobooks, and new narrators.
- Problem (worsening): rejection emails, chapters re-recorded, launch delayed, and each fix (normalising) breaks another spec (noise floor).
- Promise: *I help indie authors narrating their own audiobooks whose files keep failing ACX on noise floor or RMS get every chapter passing ACX QA in one weekend.*
- Format: 20–25 page PDF, presets/macros for Audacity, Reaper and Audition (GarageBand notes), room and mic checklist, chapter consistency sheet, pre-submission QA spreadsheet.
- Price: $39 / $59.
- Where: r/audiobooks (232k), r/VoiceActing (41–67k), r/selfpublish, the Audacity forum, author Facebook groups (sizes unverified).
- Competition: $497 course; free forum help; checker tools.
- Score: `4 4 5 5 5 | 3 4 4 5 5 5` → **85.6**.
- Risks: AI narration (e.g. Amazon's Virtual Voice) may shrink self-narration **[unverified trend]**. ACX could change its specs. Never promise acceptance: ACX also judges "overall quality".

**A2. Freelance mixer business kit (contract, revision policy, pricing calculator, intake form, client stem-prep guide, Notion CRM)**
- Promise: *I help freelance mix engineers on SoundBetter or Fiverr whose projects drag into round 6 of free revisions get a contract, revision policy and pricing sheet clients sign before day 1, this week.*
- Price: $29–39.
- Where: r/mixingmastering, r/audioengineering, Gearspace (strict promotion rules).
- Competition: free Violet Recording guides; SoundBetter product.
- Score: `4 3 4 4 5 | 3 4 3 4 5 3` → **75.4**. Contract templates are legal documents, so add a "not legal advice" note (F6 3).

**A3. Streaming loudness and delivery spec sheet** (rejected)
- Score: `2 2 3 3 4 | 2 4 2 5 5 5` → **58.0**, fails the gate on D1.
- It's a want, and Spotify's own page answers it for free.

**A4. Podcast vocal chain + remote-guest SOP for company (B2B) podcasts**
- Promise: *I help marketing managers running a company podcast whose remote-guest audio sounds like a phone call get consistent, broadcast-ready episodes with presets and a one-page guest SOP in one afternoon.*
- Price: $49. Where: r/podcasting (163–194k), LinkedIn.
- Competition: $95 Gumroad pack; MRC presets.
- Score: `3 2 4 3 5 | 3 4 4 5 4 5` → **69.8**. The pain doesn't get worse over time.

**A5. Church X32/Wing volunteer kit (stable scene file, one-page Sunday checklist, feedback-fix flowchart, 4-week volunteer training plan)**
- Promise: *I help volunteer sound leads at small churches running an X32 or Wing whose Sunday feedback draws complaints every week get a stable scene and a one-page checklist new volunteers can run within 2 Sundays.*
- Price: $39–49.
- Where: r/livesound, church-tech Facebook groups (sizes unverified).
- Competition: Drew Brashler; free QSC training ([AV Network](https://avnetwork.com/news/qsc-premieres-house-of-worship-audio-training-series)).
- Score: `4 3 4 5 5 | 3 3 4 3 4 5` → **75.4**. F4 is 3 because the owner's live-sound experience isn't stated in the brief. Confirm it.

**A6. Atmos deliverables for stereo mix engineers (headphone/binaural workflow in Logic or Pro Tools, stems-to-objects template, delivery checklist)**
- Promise: *I help stereo mix engineers whose clients now ask for Dolby Atmos deliverables get a headphone-based workflow and delivery checklist to ship a first paid Atmos mix in 2 weeks.*
- Price: $79.
- Competition: $10 PDF (2022), courses $20–$1,495, free Production Expert templates.
- Score: `3 3 4 4 4 | 4 3 3 4 3 5` → **70.2**. Uses the owner's spatial skills, but the pain is moderate.

**A7. Ambisonics quick-start for indie VR/360/game creators (Reaper + IEM template, FOA/HOA, platform delivery checklist)**
- Promise: *I help indie VR/360 creators whose spatial audio collapses after upload get a working Reaper + IEM template and a delivery checklist in one day.*
- Price: $39.
- Competition: free university and IEM tutorials.
- Score: `3 2 4 4 4 | 3 2 3 5 4 5` → **65.4**. The owner's rarest skill, but the weakest market: small, academic, used to free material.

**A8. "My mix sounds bad in the car" translation kit** (rejected)
- Score: `2 2 3 3 4 | 2 4 2 5 4 5` → **57.4**, fails the gate on D1. Hobby pain, crowded free content.

**A9. Voice audio fix for online course creators and YouTubers (free room fixes, one preset per DAW or Descript, recording SOP)**
- Promise: *I help online course creators whose students complain about echoey, uneven lesson audio get clean, consistent voice audio in one afternoon.*
- Price: $29.
- Score: `3 3 4 4 5 | 4 3 3 5 5 5` → **74.0**.

**A10. Indie film dialogue cleanup + festival/distributor QC deliverables (dialogue chain, M&E and stems checklist, loudness specs)**
- Promise: *I help indie filmmakers whose festival or distributor QC is rejecting the mix get deliverable-ready dialogue and M&E stems in one week.*
- Price: $59.
- Where: r/Filmmakers, r/editors (sizes not checked).
- Score: `4 4 4 4 4 | 3 3 3 4 4 5` → **74.8**. F4 is 4: depth in film post-production isn't stated in the brief.

---

## 3. Java

### 3.1 Where buyers gather

| Community | Size | Source |
|---|---|---|
| r/java | ~368–395k (strict about self-promotion **[check rules]**) | [GummySearch](https://gummysearch.com/r/java/) |
| r/learnjava | ~182–191k | [GummySearch](https://gummysearch.com/r/learnjava) |
| r/javahelp | ~105k | [GummySearch](https://gummysearch.com/r/javahelp/) |
| Java job market | Mid-level $114–141k, senior $141–170k (recruiter estimate) | [Motion Recruitment](https://motionrecruitment.com/it-salary/java) |
| Other channels | Medium, dev.to, newsletters, LinkedIn, Spring community | none |

### 3.2 Recurring pain and deadlines (evidence)

- **Spring Boot 3.5 open-source support ended 30 Jun 2026.** The final OSS release was 3.5.16 ([spring.io](https://spring.io/blog/2026/06/25/spring-boot-3-5-16-available-now/), [HeroDevs](https://www.herodevs.com/blog-posts/spring-boot-3-5-is-officially-end-of-life-here-is-what-that-means-for-teams-still-running-it)). Sources disagree on when 4.0 support ends: Dec 2026 or mid-2027 ([endoflife.ai](https://endoflife.ai/article-spring-june-30-eol-wave), [eosl.date](https://eosl.date/eol/product/spring-boot/)).
- **Spring Boot 4 upgrade pain:**
  - Jackson 3 is "the biggest breaking change" and "most likely to break your app silently".
  - Spring Security 7 defaults change.
  - Jackson and Hibernate major versions come along with the upgrade.
  - Sources: [ITNEXT](https://itnext.io/migrating-to-spring-boot-4-challenges-and-best-practices-ae57955a58e3), [dev.to](https://dev.to/aytronn/spring-boot-40-migration-guide-for-production-teams-what-actually-breaks-and-how-to-upgrade-safely-22me), [levelup](https://levelup.gitconnected.com/surviving-a-big-bang-java-upgrade-jackson-2-3-hibernate-6-7-and-spring-boot-3-4-1b55252eb2f9).
  - Free AI skill files for this migration already exist ([skills.sh](https://skills.sh/ajaywadhara/agent-skills/spring-boot-4-migration)).
- **Java 8 still in production.** Red Hat OpenJDK 8 enters extended support in Nov 2026 ([Red Hat checklist](https://www.redhat.com/rhdc/managed-files/su-5-upgrade-openjdk-8-checklist-3095461OM-202511-en_0.pdf)). Java 8 "still holds a significant share" ([Grandlinux, citing Azul](https://www.grandlinux.com/en/blogs/java-8-eol.html)).
- **Oracle Java licensing:**
  - Since 2023 the price is per employee, not per user.
  - Audits are claimed to be about 3× more frequent ([Redress](https://redresscompliance.com/oracle-java-audit-defence-2026-playbook.html), [OLE](https://oraclelicensingexperts.com/services/oracle-java-audit-defense/)). **Vendor claims, unverified.**
- **JVM on Kubernetes, OOMKilled:**
  - The usual cause is a container limit equal to -Xmx, plus metaspace from Spring apps ([DZone](https://dzone.com/articles/java-pod-oomkill-kubernetes), [OneUptime](https://oneuptime.com/blog/post/2026-02-09-oomkilled-tuning-memory-limits-jvm/view), [pulse.bot "invisible OOMKill"](https://www.pulse.bot/devops/news/the-invisible-oomkill-why-your-java-pod-keeps-restarting-in-kubernetes-47541cb5-b306-4528-845a-ff6d690dc9c3/)).
  - Questions about it show up on Q&A sites ([Codemia](https://codemia.io/knowledge-hub/path/kubernetes_simple_springboot_app_oomkilled)).
- **Job market:** mixed. Spring Boot is still the most requested skill, but postings are falling ([Misujob](https://misujob.com/reports/java/2026-06/), [Scanrole](https://us.scanrole.com/roles/java-developer/)).

### 3.3 Existing paid products and prices

| Product | Price | Proof | Source |
|---|---|---|---|
| Grokking the Spring Boot Interview (Javin Paul) | $19.90 | **813 sales** shown (snippet) | [Gumroad](https://javinpaul.gumroad.com/l/hrUXKY) |
| Grokking the Java Interview | $19.90 | "1,122+ copies on Gumroad" (author's own claim) | [Medium](https://medium.com/javarevisited/for-gumroadday-grokking-the-java-interview-books-are-pay-what-you-want-1-minimum-today-only-4a92b67c382e) |
| Java + Spring + SQL interview bundle | $49.90 (list price $149.40) | — | [Gumroad](https://javinpaul.gumroad.com/l/java-interview-bundle) |
| Cheap interview PDFs | $1.99 | Price race to the bottom | [Gumroad](https://codewithnik.gumroad.com/l/java-interview-prep) |
| Enthuware OCP 21 mock exams | $9.99 for 1,200+ questions | Strong low-price incumbent | [Enthuware](https://enthuware.com/129-popular-mock-exams) |
| Udemy 1Z0-830 practice tests | $39.99–$64.99 list | Most have under 30 ratings | [Udemy](https://www.udemy.com/course/ocp-java-se-21-developer-exam-1z0-830-practice-exams/) |
| "JDK 8 onwards" book (Leanpub) | Price not shown | Migration market exists | [Leanpub](https://leanpub.com/jdk8onwards) |
| Spring Boot extended commercial support | Enterprise $$$ | Shows budget for EOL pain | [HeroDevs](https://www.herodevs.com/blog-posts/spring-boot-3-5-eol-what-the-migration-really-takes) |

### 3.4 Java ideas (8)

**J1. Spring Boot 3.5 → 4.x upgrade playbook (Jackson 3, Security 7, modularisation; OpenRewrite recipe order; test strategy; AI-agent prompt and CLAUDE.md pack)**
- Promise: *I help Java teams still on Spring Boot 3.5, whose open-source support ended on 30 June 2026 and whose CVE scanners now flag it, get a staged upgrade to 4.x with the Jackson 3 and Security 7 traps pre-mapped in 2 sprints.*
- Price: $49 / $199 team.
- Where: r/java (strict), r/SpringBoot, dev.to, LinkedIn.
- Competition: many free guides; free agent skills; paid commercial support.
- Score: `4 5 4 4 4 | 4 4 3 5 4 5` → **83.0**.

**J2. Java 8/11 → 21/25 migration checklist + jdeps/jdeprscan scripts + test plan**
- Promise: *I help teams still on Java 8 or 11 whose vendor support is ending get a dependency-driven migration plan in 2 weeks.*
- Price: $49.
- Competition: free Red Hat checklist; Leanpub book.
- Score: `3 4 4 4 3 | 4 3 3 5 4 5` → **73.4**.

**J3. Oracle Java licensing exit kit (scripts that find Oracle JDK installs, OpenJDK distribution comparison, swap runbook)**
- Buyer: IT and software-asset managers.
- Promise: *I help IT managers whose company received an Oracle Java licensing letter get every Oracle JDK install inventoried and a tested OpenJDK swap plan in 10 days.*
- Price: $149.
- Where: r/sysadmin and IT manager communities (sizes not checked).
- Competition: consultancies' free white papers and paid services.
- Score: `4 5 4 5 4 | 5 2 3 3 4 3` → **79.8**. F4 3 and F6 3: the technical half is his field, the licensing and legal half is not. Must say "not legal advice".

**J4. JVM-on-Kubernetes memory kit (OOMKilled decision tree, sizing calculator spreadsheet, flags cheat sheet, Grafana/Prometheus panel JSON)**
- Promise: *I help backend developers whose Spring Boot pods keep getting OOMKilled (exit 137) despite "low heap" get a right-sized memory configuration and alerting in one afternoon.*
- Price: $29.
- Where: r/java, r/kubernetes, r/devops (sizes not checked), dev.to.
- Competition: many free blogs.
- Score: `4 4 5 5 5 | 4 3 3 4 5 5` → **83.4**. F4 is 4: Kubernetes production experience is assumed, not stated.

**J5. Senior Java/Spring interview kit (for laid-off seniors with an interview in 2 weeks)**
- Price: $29.
- Score: `4 4 4 3 4 | 3 3 2 5 4 4` → **72.6**. Demand is proven (813 sales) but the market is crowded and generic.

**J6. OCP Java 21 (1Z0-830) cram sheet and "trap" notes**
- Price: $19.
- Score: `3 4 4 4 4 | 2 3 2 5 4 5` → **68.6**. Enthuware at $9.99 sets the price ceiling.

**J7. AI-agent pack for legacy Java modernisation (CLAUDE.md templates, OpenRewrite + agent workflow, review checklists)**
- Price: $29.
- Score: `3 3 3 3 4 | 3 3 2 4 5 5` → **63.4**. Free skill files compete; the outcome is vague.

**J8. Spring Security 7 configuration cookbook (12 tested setups: JWT resource server, OAuth2 login, method security, CORS)**
- Promise: *I help Spring developers whose APIs started returning 401/403 after a Security upgrade get working, tested configurations in one afternoon.*
- Price: $39.
- Score: `4 3 4 4 4 | 4 3 3 4 4 5` → **74.8**.

---

## 4. All ideas ranked

| Rank | ID | Idea | Score | Gate |
|---|---|---|---|---|
| 1 | A1 | ACX Pass Kit | 85.6 | pass |
| 2 | N5 | Go-live CSV import kit | 84.6 | pass |
| 3 | N11 | EDI trading-partner onboarding kit | 84.6 | pass |
| 4 | J4 | JVM-on-Kubernetes memory kit | 83.4 | pass |
| 5 | J1 | Spring Boot 3.5→4 upgrade playbook | 83.0 | pass |
| 6 | N2 | Saved search formula library | 81.2 | pass |
| 7 | N1 | SOAP→REST / OAuth 2.0 migration kit | 80.0 | pass |
| 8 | N6 | Renewal negotiation playbook | 79.8 | pass |
| 8 | J3 | Oracle Java licensing exit kit | 79.8 | pass |
| 10 | N7 | SuiteScript governance cookbook | 79.4 | pass |
| 11 | N4 | Advanced PDF template pack | 79.0 | pass |
| 12 | N12 | Inherited-account health check | 78.8 | pass |
| 13 | N9 | EU e-invoicing readiness kit | 78.6 | pass |
| 14 | N10 | Month-end close pack | 76.6 | pass |
| 15 | N3 | SuiteQL query pack | 75.4 | pass |
| 15 | A2 | Freelance mixer business kit | 75.4 | pass |
| 15 | A5 | Church X32/Wing volunteer kit | 75.4 | pass |
| 18 | A10 | Indie film dialogue + QC deliverables | 74.8 | pass |
| 18 | J8 | Spring Security 7 cookbook | 74.8 | pass |
| 20 | A9 | Course-creator voice audio fix | 74.0 | pass |
| 21 | J2 | Java 8/11 → 21/25 migration | 73.4 | pass |
| 22 | J5 | Senior Java interview kit | 72.6 | pass |
| 23 | A6 | Atmos deliverables for stereo mixers | 70.2 | pass |
| 24 | A4 | B2B podcast vocal chain + guest SOP | 69.8 | pass |
| 25 | J6 | OCP 21 cram sheet | 68.6 | pass |
| 26 | A7 | Ambisonics VR/360 quick-start | 65.4 | pass |
| 27 | J7 | AI-agent legacy Java pack | 63.4 | pass |
| — | N8 | Java→NetSuite career guide | 61.8 | **fail D1** |
| — | A3 | Loudness spec sheet | 58.0 | **fail D1** |
| — | A8 | Mix translation kit | 57.4 | **fail D1** |

**Note on the model:**
- Reach (F2, 10%) is the main thing that separates the B2B NetSuite ideas, but at its current weight it rarely changes the ranking. For a *first* sale, reach matters more than the weights show, which is why the first-product pick goes beyond the raw score.
- Consider adding a "warm audience" factor (does the operator already know buyers?) to the rubric.

## 5. Open questions and things to verify before building

1. **Test account:** does the owner have a NetSuite account he may legally use to build and test commercial content (a partner or SuiteCloud developer account)? **[unverified]**
2. **Self-promotion rules** for r/Netsuite, the NetSuite Professionals Slack, r/audiobooks, r/VoiceActing and r/java. Read the sidebar or pinned rules before posting (not readable from this session).
3. **Live counts and prices:** re-check member counts and Gumroad/Udemy figures on the live pages; this session's network blocked direct fetches.
4. **ACX specs:** confirm the official ACX submission requirements, and whether AI narration (Virtual Voice) is shrinking self-narration.
5. **Trademarks:** "NetSuite", "Oracle", "ACX", "Dolby Atmos" and "Spring" may appear only descriptively ("for NetSuite"), never as brand names, and no logos.
6. **Whop for B2B:** check whether Whop receipts or invoices meet company expense and VAT-ID needs. Team-license tiers can be set up as separate plans.
7. **Search trends** were not checked (no Google Trends access). The only signal is indirect: many vendor SEO articles dated 2026 on SOAP→REST, KSeF and Spring Boot 4 point to commercial interest.
