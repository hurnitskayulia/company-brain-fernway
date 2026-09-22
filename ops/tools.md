---
owner: Hana
last_reviewed: 2026-09-22
source: Company context pack, section 3
---

# Tools

What each tool is for. No data, exports, or credentials from any of these live in this repo — see [RULES.md](../RULES.md).

| Tool | Purpose |
|---|---|
| Slack | Main channel for everything. Most decisions happen in threads. |
| Notion | Legacy pages, mostly written in the company's first six months and not maintained since. **Not a source of truth.** Page count: see migration note below. |
| HubSpot | CRM and sales pipeline. |
| Linear | Engineering tickets. |
| Intercom | Customer support inbox. |
| Stripe | Billing and invoices. |
| Google Workspace | Docs, shared drive, calendars. |
| Metabase | Dashboards over the production database. Shared read-only login — credentials are in 1Password. |
| n8n | Ivan's internal automations instance — see [engineering/automations.md](../engineering/automations.md). |
| 1Password | Where secrets live. |

GAP: "how to get access" and a per-tool owner aren't specified in the source material for most of these tools (Hana is named as the general tooling admin, but tool-by-tool ownership isn't broken out). Hana to fill in.

GAP: **GitHub** isn't in Fernway's current tool list per the source material — this repo itself has no documented admin owner, access list, or visibility setting. Hana, as tooling admin, to chase down an owner.

## Migrating from Notion

~60 pages, as of 2026-09-22, taken from the company context pack and not yet verified. Source of truth: Notion. None have been triaged yet. Don't copy anything from Notion into this repo until that page's real-world owner confirms the content is still current — see [RULES.md](../RULES.md) rule 12.

GAP: verify the page count against Notion and update the date. Routed to brain owner (Hana, proposed).
