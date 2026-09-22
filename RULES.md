---
owner: Hana (proposed; Mara to confirm)
last_reviewed: 2026-09-22
source: Fernway company brain design doc, section 3
---

# Contribution rules (human and AI)

These are hard rules. They apply to every page in this repo, and to every AI agent working in it.

1. **No secrets.** Never commit passwords, API keys, tokens, or logins — including the Metabase login and any n8n keys. Write "stored in 1Password" instead.
2. **No customer data.** No customer contact names, phone numbers, emails, staff lists, CSVs, ticket text, or billing records. Don't name customer accounts; refer to "the HubSpot record."
3. **No exports.** Never commit exports from HubSpot, Stripe, Intercom, Metabase, n8n, or the production database.
4. **No compensation or individual HR information.**
5. **Every fact has a source.** Each page lists its owner and its source: a person or a link to a public Slack thread. Nothing sourced from a DM goes in.

**Process-page exception.** README.md, RULES.md and decisions.md describe the brain's own rules and mechanics, not facts about the company. They may cite this design document as their source.

**Seed-source exception.** Pages created in the initial build (2026-09-22) may cite "Company context pack" as their source. This exception expires on 2026-12-21. By then, each page owner replaces it with a person or a public Slack thread link, or the page is flagged as stale under the 90-day rule. No new pages may use this source.

6. **Don't resolve conflicts.** If two sources disagree, write both, add an entry to `decisions.md` naming the decider, and link to it from the page.
7. **Don't invent anything.** No processes, numbers, owners, or tools that aren't sourced. If something is missing, mark it `GAP:` and name who has to fill it.
8. **Use Fernway's terms exactly as defined in `glossary.md`.** "Account" and "venue" are never interchangeable.
9. **Link rather than copy live numbers.** Don't copy numbers that live in a tool; either link to the tool or add an "as of [date]" stamp.
10. **Every page has front-matter:** owner, contributor (optional), last_reviewed, source. A page without an owner doesn't get merged.

**Owner and contributor.** The owner is the folder owner. They are accountable for the page staying current, approve PRs to it and chase the contributor when it goes stale. The contributor is optional: the person who holds the knowledge and writes or updates the content. A page without an owner doesn't get merged; a page without a contributor is fine.

11. **Changes go through a pull request,** approved by the folder owner. AI agents may open PRs but never merge them.
12. **Migrating from Notion:** copy nothing until the page owner confirms the content is current.
13. **Write in English.**
