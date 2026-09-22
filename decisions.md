---
owner: Hana (proposed; Mara to confirm)
last_reviewed: 2026-09-22
source: Fernway company brain design doc, section 4
---

# Open decisions

This is the one place contradictions live. If a page disagrees with itself or with another page, it links here instead of picking a side. Nothing on this list gets resolved by editing a page — it gets resolved in a public Slack channel, and then this entry (and the linked pages) get updated within the week.

Status key: **Open** — not yet decided. **Decided** — resolved; see the linked page for the outcome.

| # | Decision | Decider | Status |
|---|---|---|---|
| 1 | [Lead qualification target: 24h vs 48h](#1-lead-qualification-target) | Sofia | Open |
| 2 | [Activation: which definition is "the" definition](#2-activation) | Mara, with input from Sofia, Lukas, Ivan | Open |
| 3 | [When the two legacy €29/venue accounts are told and migrated](#3-legacy-pricing-migration) | Mara | Open |
| 4 | [What may be pasted into the Claude support-drafts trial](#4-claude-trial-paste-rules) | Ivan (customer-data owner), confirmed by Mara | Open |
| 5 | [New-hire account access: day one vs week two](#5-new-hire-account-access) | Mara, with Hana | Open |
| 6 | ["Live in under a day" pitch vs 1–3 day typical T2L](#6-t2l-claim-vs-target) | Mara and Sofia on the claim; Lukas on the target | Open |
| 7 | [Whether n8n stays in Ivan's own instance](#7-n8n-instance) | Ivan and Mara | Open |
| 8 | [Who is brain owner](#8-brain-owner) | Mara | Open |

---

### 1. Lead qualification target

Sofia's stated rule is that inbound leads must be qualified within 24 hours. Priya's actual practice, quietly accepted by the team, is 48 hours in busy weeks. No one has decided which is the real rule.

Linked from: [sales/inbound-lead.md](sales/inbound-lead.md).

### 2. Activation

Three different definitions are in active use and nobody has picked one — see [glossary.md](glossary.md#activation--open-decision) for all three and their sources.

Linked from: [glossary.md](glossary.md).

### 3. Legacy pricing migration

Two accounts are still on 2024-era €29/venue pricing and haven't been migrated to the current €39/venue rate. Sofia wants this fixed before the next raise; Mara hasn't set a date for telling them.

Linked from: [company/pricing.md](company/pricing.md).

### 4. Claude trial paste rules

The team is trying Claude for support draft replies. No rules exist yet for what may be pasted into it, which sits in tension with the existing rule that customer data stays in HubSpot/Stripe/the production database and isn't exported into AI tools.

Linked from: [support/ai-drafts.md](support/ai-drafts.md).

### 5. New-hire account access

The Notion onboarding checklist says a new hire gets all accounts on day one. In practice, most people wait until week two.

Linked from: [people/new-hire.md](people/new-hire.md).

### 6. T2L claim vs target

Fernway's pitch is "live in under a day." The onboarding flow that's actually run produces a typical time-to-live of 1–3 days.

Linked from: [company/overview.md](company/overview.md), [onboarding/t2l.md](onboarding/t2l.md).

### 7. n8n instance

All of Fernway's internal automations run in Ivan's personal n8n instance. Whether that stays the setup hasn't been decided.

Linked from: [engineering/automations.md](engineering/automations.md).

### 8. Brain owner

Hana is proposed as brain owner. Mara has not yet confirmed this.

Linked from: [README.md](README.md), [RULES.md](RULES.md).
