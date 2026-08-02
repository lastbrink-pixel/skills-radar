# 🛰️ Skills Radar

A curated, weekly-updated catalog of **genuinely useful agent skills** — for Claude Code, Codex, Gemini CLI, and any agent that reads `SKILL.md`. No dumps of every repo on GitHub: every entry here was checked by a human, described in one honest line, and tagged by the Scrum role it helps.

**📬 Get the weekly digest:** hit **Watch → Custom → Releases** on this repo — GitHub will email you the top finds every week. Works for any team member, no signup, no bot.

## How entries get here

A weekly job scans [skills.sh](https://skills.sh), GitHub, and community lists for new skills, filters out junk (dead READMEs, spam authors, empty wrappers), and proposes candidates. A human reviews every candidate before it lands in the catalog. Statuses: `✅ approved` · `🆕 new this week` · `🎒 in a role kit`.

## Catalog

### 🧠 Decision quality

| Skill | What it actually does | Roles | Installs |
|---|---|---|---|
| [council](https://skills.sh/warpdotdev/common-skills/council) `warpdotdev/common-skills` | Karpathy-style LLM Council: several agents (different models when available, different perspectives otherwise) investigate the same question independently, cross-review, then synthesize one recommendation | BA, PO, DEV | 16.3K |
| [llm-council](https://github.com/okjpg/llm-council) `okjpg` | 5 AI advisors debate your decision with peer review and synthesis — closest to Karpathy's original methodology | BA, PO | — |
| [judge-with-debate](https://skills.sh/neolabhq/context-engineering-kit/judge-with-debate) `neolabhq/context-engineering-kit` | Structured judge + debate loop for evaluating outputs before shipping them | QA, DEV | 947 |

### 🗣️ Communication

| Skill | What it actually does | Roles | Installs |
|---|---|---|---|
| [empathy-in-action](https://github.com/lastbrink-pixel/empathy-in-action) `lastbrink-pixel` | Empathy through action, not words: the assistant picks up the rational load when emotions block reason — mirrors the user's register, never fakes capabilities, ticking-clock mode for live incidents | ALL | new |
| [negotiation-voss-tactical-empathy](https://skills.sh/santos-sanz/lifeskills/negotiation-voss-tactical-empathy) `santos-sanz/lifeskills` | Chris Voss negotiation techniques (tactical empathy, calibrated questions) applied to your negotiation prep | PO, SM | 43 |

### 📋 Discovery & requirements

| Skill | What it actually does | Roles | Installs |
|---|---|---|---|
| [empathy-map](https://skills.sh/owl-listener/designer-skills/empathy-map) `owl-listener/designer-skills` | Builds a UX empathy map (says/thinks/does/feels) from your user research notes | BA, PO | 943 |
| [customer-empathy](https://skills.sh/rameerez/claude-code-startup-skills/customer-empathy) `rameerez/claude-code-startup-skills` | Digs into customer pains and jobs-to-be-done before you commit to building | PO, BA | 108 |

### 🛠️ Engineering

| Skill | What it actually does | Roles | Installs |
|---|---|---|---|
| [react-best-practices](https://skills.sh/vercel-labs/agent-skills/react-best-practices) `vercel-labs/agent-skills` | React/Next.js performance guidelines straight from Vercel engineering | DEV | 185K |
| [document skills](https://github.com/anthropics/skills) `anthropics/skills` | Official Anthropic skills for producing real .docx / .xlsx / .pptx / .pdf artifacts | ALL | 100K+ |
| [skill-creator](https://github.com/anthropics/skills) `anthropics/skills` | Meta-skill: builds new skills with test runs, benchmarks, and an iteration loop — how the skills in this catalog get made | ALL | 100K+ |

### 🧰 Memory & context

| Skill | What it actually does | Roles | Installs |
|---|---|---|---|
| [agentmemory](https://github.com/rohitg00/agentmemory) `rohitg00` | 15 persistent-memory skills (remember / recall / handoff / commit-context) so your agent survives session restarts | ALL | — |

## Role kits

Skills from this catalog are being assembled into installable **role kits** for Scrum teams (ba-kit, po-kit, sm-kit, dev-kit, qa-kit) — one command installs the whole set for your role. Coming at [lastbrink-pixel/role-kits](https://github.com/lastbrink-pixel/role-kits).

## Contributing

Found a skill that deserves a spot? Open an issue with the link and one line on why it's genuinely useful. "It exists" is not a reason; "it saved me an hour this week" is.

## License

MIT — the catalog data (`catalog.json`) is free to reuse.
