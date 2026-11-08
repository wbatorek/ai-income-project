# Tax and legal setup

> Not tax advice. These are working notes to bring to a tax adviser. Rules change, so check
> everything marked **[verify]** before relying on it.

## Current setup (as of Nov 2026)

- **Selling entity:** Noventa Tech LLC, a US LLC set up through Taxhackers.
- **Owner:** Wojciech Bątorek, the only member, not a US person.
- **Poland:** deregistered. The owner no longer considers himself a Polish tax resident.
- **Location:** currently living in Thailand.
- **US income:** none so far. The working assumption is that the LLC pays no US tax on income
  from outside the US.

> This replaces the Poland-based assumptions in
> [`research/self-running-ai-system.md`](../research/self-running-ai-system.md), section on tax.

## How a foreign-owned, single-member LLC is usually taxed

1. **Federal income tax.** A single-member LLC owned by a foreign person is normally a
   *disregarded entity*. It owes US federal income tax only on income *effectively connected
   with a US trade or business* (ECI). Selling digital products online while you work from
   outside the US, with no US office, employees or dependent agents, is usually **not** ECI.
   A US customer buying the product does not by itself create US tax. **[verify with adviser]**
2. **Annual filing is still required, even with no tax due:** **Form 5472 plus a pro forma
   Form 1120** every year. Penalties for missing it are high (from $25,000). Check whether
   Taxhackers handles this. **[verify]**
3. **State taxes.** These depend on the state the LLC is registered in (annual report or
   franchise fees, e.g. Wyoming, New Mexico, Delaware). **[verify which state]**
4. **US sales tax on digital products.** Many US states tax digital goods and apply
   "economic nexus" thresholds. Selling through a **merchant of record** (Whop, Gumroad,
   Lemon Squeezy, Paddle) moves collecting and paying this tax to the platform. Selling
   directly through Stripe leaves it with us.
5. **EU VAT and UK VAT** on digital products sold to consumers. A merchant of record handles
   this too. Without one, a non-EU seller must register for non-Union OSS from the first euro.
   This is the main reason to **always sell through a merchant of record**.

## Personal tax: where the money finally gets taxed

The LLC being tax-free in the US does **not** mean the income is tax-free. Because the LLC is
disregarded, its profit usually counts as the owner's personal income, taxed wherever he is
**tax resident**.

- **Thailand.** Someone who spends **180+ days** in Thailand in a calendar year is a Thai tax
  resident. Since **1 Jan 2024**, Thailand taxes foreign-source income **brought into
  Thailand** by residents, whenever it was earned. Rules on timing and exemptions were still
  changing. **[verify, important]**
- **Poland.** Deregistering doesn't automatically end Polish tax residency. Poland looks at
  the *centre of vital interests* (family, home, economic ties) and at 183+ days spent there.
  Keep evidence of residency elsewhere, such as a certificate of tax residency from another
  country. **[verify]**
- **Countries with no personal tax residency anywhere** ("perpetual traveller") are a
  grey area. Platforms, banks and future tax authorities may still ask for proof of
  residency.

## Practical checklist

- [ ] Confirm the LLC has an **EIN** and a US business bank account (Mercury, Relay or Wise Business)
- [ ] Register on Whop (and other platforms) **as Noventa Tech LLC** and submit **Form W-8BEN-E**
      (or W-9, depending on how the disregarded LLC is classified on the platform's form) **[verify]**
- [ ] Confirm who files **Form 5472 + 1120** each year and the deadline (normally 15 April)
- [ ] Sell only through **merchant-of-record** platforms, so sales tax and VAT are handled
- [ ] Decide and document **personal tax residency** (Thailand 180-day rule, Poland ties)
- [ ] Ask an adviser about remitting money to Thailand (timing, amounts, exemptions)
- [ ] Keep records of every sale, payout and expense, by month

## Questions for the tax adviser

1. Is anything we do likely to count as US effectively connected income (ECI)? What would change that
   (for example a US contractor, or a US warehouse for physical goods)?
2. Given the days I spend in Thailand, am I a Thai tax resident? How is LLC profit treated when I
   bring money into Thailand?
3. Is there any remaining risk of Polish tax residency, and what proof should I keep?
4. Do I need a certificate of tax residency anywhere for platforms or banks?
5. What exactly does Taxhackers file each year, and what is left for me?
