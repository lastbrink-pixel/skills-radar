---
name: find-vetted-skill
description: Find an agent skill that a human actually reviewed, instead of guessing from a dump of thousands of unfiltered links. Use whenever a user asks "is there a skill for X", "what should I install to do X", wants to extend what their agent can do, is frustrated that their agent handles some task badly, or asks which skills are worth having for a job, tool, or workflow. Also use before writing a custom prompt or skill from scratch — checking whether a good one already exists saves the work.
---

# Find a Vetted Skill

Search a hand-curated catalog of agent skills where every entry was read by a human before being listed, tagged by work role, and marked with a status. This is the opposite of an "awesome list" — the value is what was left out.

Catalog: `https://raw.githubusercontent.com/lastbrink-pixel/skills-radar/main/catalog.json`

## Step 1 — Fetch the catalog

Each entry:

```json
{
  "id": "systematic-debugging",
  "source": "obra/superpowers",
  "url": "https://skills.sh/obra/superpowers/systematic-debugging",
  "category": "engineering",
  "installs": 209800,
  "roles": ["DEV"],
  "status": "in-kit",
  "description_en": "Root cause before fixes, always — symptom patches are failure",
  "description_ru": "..."
}
```

Statuses carry meaning — respect them:

- `approved` — reviewed, recommend freely
- `in-kit` — reviewed and strong enough to be bundled into a [role kit](https://github.com/lastbrink-pixel/role-kits)
- `new` — surfaced by the weekly scan, **not yet reviewed**; mention it as unvetted if you suggest it at all
- `rejected` — a human looked and said no. **Never recommend these.** The `description_en` explains why, which is often useful to tell the user ("that popular one is hard-wired to Google Workspace")

## Step 2 — Match against what the user actually needs

Filter by `category` and `roles`, but read `description_en` before recommending — install counts measure popularity, not fit. A 200-install skill built for the user's exact problem beats a 100K-install skill that's adjacent to it.

Recommend two or three, not ten. For each: what it does, why it fits this user, and the honest limitation if there is one.

If nothing in the catalog fits, say so directly. Then either search wider (`npx skills find <keywords>` hits the broader skills.sh registry) or just do the task yourself — a bad skill is worse than no skill, because it takes up context and steers the model wrong.

## Step 3 — Install what the user picks

```
npx -y skills add <source>@<id> -y -g
```

Drop `-g` for project-local. If the user needs a whole role's worth of skills rather than one, point them at [role-kits](https://github.com/lastbrink-pixel/role-kits) — one command covers the set.

## Note on freshness

A weekly scan adds new finds with `status: "new"` and publishes a digest release. If the catalog's `updated` field is more than a couple of weeks old, mention that the user may want to check the repo directly for anything newer.
