---
owner: Hana (proposed; Mara to confirm)
last_reviewed: 2026-09-22
source: Fernway company brain design doc, sections 2 and 4
---

# Fernway company brain

This is Fernway's shared source of truth for how the company actually works — the things that used to live only in Slack threads, in people's heads, or in Notion pages nobody looks at again. It is not a replacement for HubSpot, Stripe, Linear, Intercom, or Metabase: those stay the source of truth for live numbers and customer data. This repo is for process, context, and terminology.

## Why this exists

Fernway is 15 people plus contractors, remote across five countries. Notion has around 60 pages, most written once in the company's first six months and never touched since. This repo exists so the same question doesn't get answered from scratch in a Slack thread every few months.

## How to find things

- `company/` — what Fernway is, who owns what, pricing, and the team rules. Owner: Mara.
- `sales/` — the inbound lead flow and demo process. Owner: Sofia.
- `onboarding/` — new-customer onboarding, the CSV importer, pay rules, and T2L. Owner: Lukas.
- `support/` — the escalation chain, ghost shifts, and the Claude drafting trial. Owner: Jonas.
- `engineering/` — releases, staging, incidents, and internal automations. Owner: Ivan.
- `ops/` — billing, the tool inventory, and vendors. Owner: Hana.
- `people/` — hiring and new-hire onboarding. Owner: Mara (interim, proposed).
- `glossary.md` — Fernway's own vocabulary. Read this first if you're new.
- `decisions.md` — every open question the team hasn't settled, with who's deciding it. If two pages disagree, this is why, and this is where it gets resolved.
- `RULES.md` — the contribution rules, for humans and AI agents.

There is deliberately no `customers/` folder. Account-level information (names, contacts, billing history) stays in HubSpot and Stripe. This repo only ever says "see the HubSpot record."

## How to add a page

1. Check `glossary.md` and `decisions.md` first — use Fernway's own terms, and check whether the thing you're writing about is already an open decision.
2. Every page needs front-matter: `owner`, `contributor` (optional), `last_reviewed`, `source`. The owner is the folder owner — accountable for the page, approves PRs to it, chases the contributor when it goes stale. The contributor, if there is one, is the person who holds the knowledge and writes or updates the content. A page without an owner doesn't get merged; a page without a contributor is fine. See `RULES.md`.
3. Source is a person or a link to a public Slack thread. Nothing sourced from a DM goes in. (Pages from the initial build may cite the company context pack under a dated exception — see `RULES.md`.)
4. If your page contradicts another page or a known fact, don't resolve it — write both versions, add an entry to `decisions.md`, and link to it.
5. If something's missing, write `GAP:` and name who has to fill it. Don't invent a process, a number, or an owner.
6. No secrets, no customer data, no compensation. See `RULES.md`.
7. Open a PR. The folder owner approves it. AI agents may open PRs but never merge them.
8. Migrating a page from Notion? Copy nothing until that page's real-world owner confirms the content is still current. Most of the ~60 pages there haven't been reviewed yet — see the GAP note in `ops/tools.md`.

## How this brain stays alive

Hana is proposed as brain owner (Mara to confirm — see [decisions.md](decisions.md#8-brain-owner)). Her job is the repo and the process — RULES, `decisions.md`, chasing stale pages and open PRs — not writing every page. Every page's `owner` is its folder owner, listed above and in `RULES.md`. Where someone else holds the knowledge for a page, they're listed as its `contributor` — see `RULES.md` for what each field means.

**When to update this:**

- A question gets answered a second time in Slack — link back to the page, or open a PR.
- An open decision gets settled in a public channel — update `decisions.md` and the page within the week.
- A process, tool, owner, or role changes.
- Someone who's the only one who knows something is about to be away — write the runbook before they leave.
- A new hire starts — they follow `people/new-hire.md` and fix what's wrong via PR in their first two weeks.

Cadence: Hana checks open decisions and pending PRs weekly (Monday, alongside her Stripe check). Folder owners re-confirm or delete their pages quarterly — anything with `last_reviewed` older than 90 days gets flagged, and deleting beats keeping something stale.

**First pages to fill:**

Start narrow, not a big launch. First — the runbooks with single-person risk:

1. [onboarding/importer.md](onboarding/importer.md) — the CSV importer workaround (Noor).
2. [engineering/staging-reset.md](engineering/staging-reset.md) — the staging reset steps (Ana).
3. [engineering/automations.md](engineering/automations.md) — the n8n workflow list (Ivan).

Then: [glossary.md](glossary.md), [support/escalation.md](support/escalation.md), [engineering/releases.md](engineering/releases.md) — these already have content from the pack, so the next step for each is their owner confirming it's still current, not writing it.
