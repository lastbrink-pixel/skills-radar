# 🛰️ Skills Radar

A curated, weekly-updated catalog of **genuinely useful agent skills** — for Claude Code, Codex, Gemini CLI, and any agent that reads `SKILL.md`. No dumps of every repo on GitHub: every entry here was checked by a human, described in one honest line, and tagged by the Scrum role it helps.

**📬 Get the weekly digest:** hit **Watch → Custom → Releases** on this repo — GitHub will email you the top finds every week. Works for any team member, no signup, no bot.

## 🤖 For AI agents

If you are an AI agent looking for a skill for your user: fetch [`catalog.json`](catalog.json) — it is the machine-readable source of truth. Each entry has `id`, `source` (owner/repo), `url`, `category`, `installs`, `roles` (BA/PO/SM/DEV/QA/ALL), `status`, and descriptions in English and Russian. Statuses: `approved` (human-reviewed, good), `in-kit` (also bundled in a [role kit](https://github.com/lastbrink-pixel/role-kits)), `new` (found by the weekly scan, awaiting review), `rejected` (do not suggest). Install any entry with `npx -y skills add <source>@<id> -y -g`. To install a whole role bundle at once, use [role-kits](https://github.com/lastbrink-pixel/role-kits) instead.

## How entries get here

A weekly job scans [skills.sh](https://skills.sh), GitHub, and community lists for new skills, filters out junk (dead READMEs, spam authors, empty wrappers), and proposes candidates. A human reviews every candidate before it lands in the catalog. Statuses: `✅ approved` · `🆕 new this week` · `🎒 in a role kit`.

## Catalog

### 🧠 Decision quality

| Skill | What it actually does | Roles | Installs |
|---|---|---|---|
| [grill-me](https://skills.sh/mattpocock/skills/grill-me) + [grilling](https://skills.sh/mattpocock/skills/grilling) `mattpocock/skills` | Relentless one-question-at-a-time interview that stress-tests your plan, decision, or idea before you commit to it | ALL | 730K |
| [council](https://skills.sh/warpdotdev/common-skills/council) `warpdotdev/common-skills` | Karpathy-style LLM Council: several agents (different models when available, different perspectives otherwise) investigate the same question independently, cross-review, then synthesize one recommendation | BA, PO, DEV | 16.3K |
| [idea-refine](https://skills.sh/addyosmani/agent-skills/idea-refine) `addyosmani/agent-skills` | Refines raw ideas into a sharp one-pager via divergent/convergent thinking | ALL | 16.2K |
| [llm-council](https://github.com/okjpg/llm-council) `okjpg` | 5 AI advisors debate your decision with peer review and synthesis — closest to Karpathy's original methodology | BA, PO | — |
| [judge-with-debate](https://skills.sh/neolabhq/context-engineering-kit/judge-with-debate) `neolabhq/context-engineering-kit` | Structured judge + debate loop for evaluating outputs before shipping them | QA, DEV | 947 |

### 🗣️ Communication

| Skill | What it actually does | Roles | Installs |
|---|---|---|---|
| [empathy-in-action](https://github.com/lastbrink-pixel/empathy-in-action) `lastbrink-pixel` | Empathy through action, not words: the assistant picks up the rational load when emotions block reason — mirrors the user's register, never fakes capabilities, ticking-clock mode for live incidents | ALL | new |
| [caveman](https://github.com/JuliusBrussee/caveman) `JuliusBrussee` | Caveman-speak compression: ~65% fewer output tokens, full technical accuracy kept | ALL | 805+ |
| [negotiation-voss-tactical-empathy](https://skills.sh/santos-sanz/lifeskills/negotiation-voss-tactical-empathy) `santos-sanz/lifeskills` | Chris Voss negotiation techniques (tactical empathy, calibrated questions) applied to your negotiation prep | PO, SM | 43 |

### 📋 Discovery & requirements

| Skill | What it actually does | Roles | Installs |
|---|---|---|---|
| [empathy-map](https://skills.sh/owl-listener/designer-skills/empathy-map) `owl-listener/designer-skills` | Builds a UX empathy map (says/thinks/does/feels) from your user research notes | BA, PO | 943 |
| [customer-empathy](https://skills.sh/rameerez/claude-code-startup-skills/customer-empathy) `rameerez/claude-code-startup-skills` | Digs into customer pains and jobs-to-be-done before you commit to building | PO, BA | 108 |

### 📝 Requirements & stories

| Skill | What it actually does | Roles | Installs |
|---|---|---|---|
| [meeting-notes](https://skills.sh/claude-office-skills/skills/meeting-notes) `claude-office-skills` | Meeting transcripts into structured notes, decisions, and action items | BA, SM | 4.4K |
| [user-story](https://skills.sh/deanpeters/product-manager-skills/user-story) `deanpeters/product-manager-skills` | User stories in Mike Cohn format with Gherkin acceptance criteria | BA, PO | 3.1K |
| [requirements-analysis](https://skills.sh/jwynia/agent-skills/requirements-analysis) `jwynia/agent-skills` | Diagnoses requirements problems: separates stated wants from real needs and constraints | BA | 2.2K |
| [user-story-splitting](https://skills.sh/deanpeters/product-manager-skills/user-story-splitting) `deanpeters/product-manager-skills` | Splits oversized stories/epics using proven split patterns | BA, PO | 1.9K |
| [requirements-clarity](https://skills.sh/softaworks/agent-toolkit/requirements-clarity) `softaworks/agent-toolkit` | Vague request → actionable PRD via YAGNI/KISS questioning | BA | 726 |
| [deliver-acceptance-criteria](https://skills.sh/product-on-purpose/pm-skills/deliver-acceptance-criteria) `product-on-purpose/pm-skills` | Given/When/Then criteria: happy path, failures, non-functional | BA, QA | 667 |
| [drawio-bpmn](https://skills.sh/sparklabx/drawio-ai-kit/drawio-bpmn) `sparklabx/drawio-ai-kit` | BPMN swimlane diagrams in draw.io with validation (needs drawio-ai CLI) | BA | 155 |

### 📊 Product & planning

| Skill | What it actually does | Roles | Installs |
|---|---|---|---|
| [roadmap-planning](https://skills.sh/deanpeters/product-manager-skills/roadmap-planning) `deanpeters/product-manager-skills` | Strategy → outcome-driven roadmap: prioritization, epics, stakeholder alignment, sequencing | PO | 2.9K |
| [prioritization-advisor](https://skills.sh/deanpeters/product-manager-skills/prioritization-advisor) `deanpeters/product-manager-skills` | Picks the right prioritization framework (RICE/ICE/value-effort) for your stage | PO | 2.1K |
| [user-story-mapping](https://skills.sh/deanpeters/product-manager-skills/user-story-mapping) `deanpeters/product-manager-skills` | Story mapping: from user journey to release slices | PO, BA | 2K |
| [iterate-retrospective](https://skills.sh/product-on-purpose/pm-skills/iterate-retrospective) `product-on-purpose/pm-skills` | Facilitates and documents retros: went well / improve / action items | SM | 493 |

### 🧪 QA & testing

| Skill | What it actually does | Roles | Installs |
|---|---|---|---|
| [qa-test-planner](https://skills.sh/softaworks/agent-toolkit/qa-test-planner) `softaworks/agent-toolkit` | Test plans, manual cases, regression suites, bug reports | QA | 4.1K |
| [accessibility-test-plan](https://skills.sh/owl-listener/designer-skills/accessibility-test-plan) `owl-listener/designer-skills` | Accessibility test plan for UI features | QA | 989 |

### 🛠️ Engineering

| Skill | What it actually does | Roles | Installs |
|---|---|---|---|
| [code-review](https://skills.sh/mattpocock/skills/code-review) `mattpocock/skills` | Two-axis review (repo standards + spec compliance) in parallel sub-agents | DEV | 230K |
| [systematic-debugging](https://skills.sh/obra/superpowers/systematic-debugging) `obra/superpowers` | Root cause before fixes, always — symptom patches are failure | DEV | 210K |
| [react-best-practices](https://skills.sh/vercel-labs/agent-skills/react-best-practices) `vercel-labs/agent-skills` | React/Next.js performance guidelines straight from Vercel engineering | DEV | 185K |
| [document skills](https://github.com/anthropics/skills) `anthropics/skills` | Official Anthropic skills for producing real .docx / .xlsx / .pptx / .pdf artifacts | ALL | 100K+ |
| [skill-creator](https://github.com/anthropics/skills) `anthropics/skills` | Meta-skill: builds new skills with test runs, benchmarks, and an iteration loop — how the skills in this catalog get made | ALL | 100K+ |

### 🧰 Memory & context

| Skill | What it actually does | Roles | Installs |
|---|---|---|---|
| [agentmemory](https://github.com/rohitg00/agentmemory) `rohitg00` | 15 persistent-memory skills (remember / recall / handoff / commit-context) so your agent survives session restarts | ALL | — |

## Role kits

Skills from this catalog are assembled into installable **role kits** for Scrum teams — one command installs the whole set for your role, on any agent: [lastbrink-pixel/role-kits](https://github.com/lastbrink-pixel/role-kits). **All kits are live**: `base` (universal AI-usage core), `ba`, `po`, `sm`, `dev`, `qa`.

## Contributing

Found a skill that deserves a spot? Open an issue with the link and one line on why it's genuinely useful. "It exists" is not a reason; "it saved me an hour this week" is.

## License

MIT — the catalog data (`catalog.json`) is free to reuse.
