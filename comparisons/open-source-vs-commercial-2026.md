# 2026 Agentic Coding Tools: Open Source vs Commercial

_Last reviewed: June 11, 2026_

This page separates agentic coding tools by licensing, product status, and maintenance activity. The older catalog mixed open-source tools, proprietary IDEs, cloud app builders, and sunsetting products together, so this file should be used as the cleaner 2026 reference.

## Status legend

- **Active**: current product worth tracking in the main catalog.
- **Active but not recent**: product may still work, but the public repo has not seen fresh commits recently.
- **Stale / questionable**: public repo has little recent maintenance and should not be treated as a top current option.
- **Sunsetting / deprecated**: historically relevant, but should not be recommended as a current first choice.
- **Renamed / replaced**: the old name should redirect to the newer product.
- **Open source**: public repo under a standard open-source license such as MIT or Apache-2.0.
- **Source-available / mixed**: source is visible, but licensing or packaging is not cleanly open source.
- **Commercial / proprietary**: closed-source SaaS, paid IDE, hosted agent, or commercial platform.

## Open-source maintenance check

Dates below are based on the latest visible commit on the primary GitHub branch checked on **June 11, 2026**. This is not the same thing as npm/package release date, company activity, or SaaS product status, but it is the best quick signal for whether the open-source repo itself is maintained.

| Tool | Latest visible GitHub commit as of June 11, 2026 | Maintenance read | Web app / hosted app relevance | Notes |
|---|---:|---|---|---|
| **Kilo Code** | June 11, 2026 | Very active | Mostly IDE/CLI/cloud surfaces, not a Bolt-style hosted app builder | Strong open-source current signal. |
| **OpenAI Codex CLI** | June 11, 2026 | Very active | No, CLI agent | Separate from commercial Codex web/app product. |
| **Goose** | June 11, 2026 | Very active | No, local desktop/CLI/API agent | Strong open-source current signal. |
| **Gemini CLI** | June 10, 2026 | Very active | No, CLI agent | Also increasingly tied to Antigravity transition docs. |
| **Dyad** | June 10, 2026 | Very active | No, local desktop app | Good project, but not what you asked for because it is local. |
| **Cline** | June 8, 2026 | Very active | No, VS Code/CLI/SDK style agent | Strong agentic coding tool, not app-builder web UI. |
| **Crush** | June 8, 2026 | Very active | No, CLI agent | Source-available FSL, not pure open source. |
| **OpenCode** | June 3, 2026 | Active | No, CLI/desktop coding agent | Very important open-source agentic coding tool. |
| **Aider** | May 22, 2026 | Active | No, CLI pair programmer | Mature and still maintained. |
| **Roo Code** | May 11, 2026 | Active, but watch status | No, VS Code extension | Recent commits exist, but public repo also contains sunsetting/transition signals, so track carefully. |
| **Wave Terminal** | May 4, 2026 | Active | No, terminal/workspace app | Maintained, but not a Bolt/Lovable-style app builder. |
| **Continue** | April 17, 2026 | Active but not very recent | No, IDE assistant | Still worth tracking, but less fresh than Cline/Kilo/Goose/Codex. |
| **Convex Chef** | March 13, 2026 | Active product, public repo not recently updated | **Yes, best hosted open-source-style app-builder match** | Still the best fit for “web app, not local,” but public repo maintenance is not as fresh as the strongest CLI/IDE agents. |
| **bolt.diy** | February 5, 2026 | Active but not recent | Sort of, but usually self-host/deploy-yourself | Best open-source Bolt clone, but less ideal than Chef for hosted web usage. |
| **app.build / appdotbuild-agent** | February 2, 2026 | **Not actively maintained** | No current managed service | README says repo is not actively maintained and the managed service was discontinued. Treat as research/reference only. |
| **Tabby** | November 26, 2025 | Stale / slower-moving | No, self-hosted code assistant | Not a current Bolt-style app builder. |
| **Pythagora / GPT Pilot** | August 13, 2025 | Stale / questionable | Not really | Open-source lineage exists, but current product should be tracked separately. |
| **PearAI** | May 16, 2025 | Stale | No, AI editor | Should not be treated as a top current open-source option unless activity resumes. |

## Practical answer for open-source web app builders

If the requirement is **open-source or source-visible, Bolt/Lovable-style, and usable as a web app rather than local-only**, the honest ranking is:

1. **Convex Chef** — best match because it has a hosted web app and backend/database awareness.
2. **bolt.diy** — best open-source Bolt clone, but generally more self-host/deploy-yourself than a polished hosted app-builder.
3. **app.build / appdotbuild-agent** — do not recommend as active; useful only as research/reference/fork material.
4. **Dyad** — very active, but local desktop, so it fails the web-app requirement.

There is still no perfect open-source hosted replacement for Lovable, Bolt.new, Base44, Replit Agent, or v0. Chef is the closest current fit, but its public repo should be watched because the last visible commit is March 13, 2026.

## Major 2026 corrections

### Firebase Studio should be moved out of the active list

Firebase Studio should be marked **sunsetting / deprecated**, not listed as a current web-based AI development platform. Google announced that Firebase Studio is sunsetting, with final shutdown planned for **March 22, 2027**. New users/workspaces are also being phased out earlier. The relevant replacement direction is **Google Antigravity** and **Google AI Studio**, while core Firebase services such as Firestore, Authentication, and App Hosting continue separately.

Recommended repo treatment:

- Keep `tools/firebase-studio.md`, but mark it `Status: Sunsetting / deprecated`.
- Move Firebase Studio from the active README category to a `Sunsetting / Deprecated` section.
- Add or prioritize `tools/google-antigravity.md`.
- Mention Google AI Studio as the migration direction for AI prototyping, but do not classify it as a repo-centric coding agent in the same way as Claude Code, Codex, Cursor, or Antigravity.

### Claude should be represented as a product family, not just “Claude Code CLI”

Claude Code is no longer just a terminal tool. The catalog should track Anthropic’s coding/dev surface as a family:

- **Claude Code CLI** — terminal coding agent.
- **Claude Code IDE integrations** — VS Code / JetBrains-style workflows where available.
- **Claude Code on the web / cloud sessions** — browser/GitHub-connected agentic coding.
- **Claude desktop app coding sessions** — local/remote sessions through Claude app surfaces where available.
- **Claude Code Review / Security** — code review and vulnerability-focused offerings for teams/enterprise.
- **Claude Cowork** — related GUI/productivity agent based on the Claude Code direction, aimed more at non-developers and file/task work than pure engineering.

Recommended repo treatment:

- Rename the mental category from **Command-line Tools** to **Terminal, IDE, and Cloud Coding Agents**.
- Keep `tools/claude-code.md`, but update it so it is not described as terminal-only.
- Add a note that Claude Code is proprietary/commercial, even though some client code or leaked/source-visible materials may exist online. It should not be listed under open source.

## Open-source / self-hostable agentic coding tools

| Tool | Category | Status | Last visible commit as of June 11, 2026 | License / openness | Repo / site | Notes |
|---|---|---|---:|---|---|---|
| **Aider** | CLI pair programmer | Active | May 22, 2026 | Open source | https://github.com/Aider-AI/aider | Mature terminal coding assistant with strong git workflow. |
| **Cline** | VS Code extension / CLI / SDK | Very active | June 8, 2026 | Open source | https://github.com/cline/cline | Autonomous coding agent with tool use and MCP support. |
| **Roo Code** | VS Code extension | Active, but watch status | May 11, 2026 | Open source | https://github.com/RooCodeInc/Roo-Code | Cline-family autonomous coding agent; track status carefully because the repo contains transition/sunsetting signals. |
| **Kilo Code** | IDE / CLI platform | Very active | June 11, 2026 | Open source, MIT | https://github.com/Kilo-Org/kilocode | Agentic engineering platform spanning VS Code, JetBrains, CLI, Slack, and cloud surfaces. |
| **OpenCode** | CLI / desktop coding agent | Active | June 3, 2026 | Open source, MIT | https://github.com/anomalyco/opencode | Major open-source terminal coding agent; should be added as its own tool page. |
| **OpenAI Codex CLI** | CLI coding agent | Very active | June 11, 2026 | Open source, Apache-2.0 | https://github.com/openai/codex | Open-source CLI client for Codex-style local coding workflows. Do not confuse with commercial Codex web/cloud product. |
| **Gemini CLI** | CLI coding agent | Very active | June 10, 2026 | Open source, Apache-2.0 | https://github.com/google-gemini/gemini-cli | Google terminal agent with Gemini models, MCP, shell/file tooling, and web grounding. |
| **Goose** | Desktop / CLI / API agent | Very active | June 11, 2026 | Open source, Apache-2.0 | https://github.com/aaif-goose/goose | Local general-purpose agent useful for code, automation, research, and MCP-style extensions. |
| **Continue** | IDE assistant / agent | Active but not recent | April 17, 2026 | Open source | https://github.com/continuedev/continue | Open-source AI coding assistant for VS Code and JetBrains; good for custom models and local/enterprise setups. |
| **PearAI** | AI editor | Stale | May 16, 2025 | Open source | https://github.com/trypear/pearai-master | Do not treat as a top current option unless activity resumes. |
| **bolt.diy** | Web app builder / Bolt clone | Active but not recent | February 5, 2026 | Open source | https://github.com/stackblitz-labs/bolt.diy | Open-source/local version of bolt-style app generation with multi-provider support. Usually more self-host/deploy-yourself than hosted app. |
| **Convex Chef** | Hosted app builder / backend-aware builder | Active product, repo not recently updated | March 13, 2026 | Open source | https://github.com/get-convex/chef | Best match for open-source-style hosted web app builder, but public repo maintenance should be watched. |
| **Pythagora / GPT Pilot** | Agentic app builder | Stale / mixed | August 13, 2025 | Open source / mixed | https://github.com/Pythagora-io/gpt-pilot | Track carefully: open-source lineage exists, but current product packaging may differ. |
| **Wave Terminal** | Terminal + AI | Active | May 4, 2026 | Open source | https://github.com/wavetermdev/waveterm | Open-source terminal with graphical widgets and AI capabilities. |
| **Dyad** | Local app builder | Very active, but local-only | June 10, 2026 | Open source | https://github.com/dyad-sh/dyad | Strong project, but not a web app. Keep separate from hosted app-builder options. |

## Source-available / mixed-license tools

| Tool | Category | Status | Last visible commit as of June 11, 2026 | Openness | Repo / site | Notes |
|---|---|---|---:|---|---|---|
| **Crush** | CLI coding agent | Very active | June 8, 2026 | Source-available, FSL-1.1-MIT | https://github.com/charmbracelet/crush | Useful terminal agent from Charmbracelet. Keep separate from pure open source because FSL is not standard MIT/Apache at release time. |
| **Tabby** | Self-hosted code assistant | Stale / slower-moving | November 26, 2025 | Open-source core / commercial options | https://github.com/TabbyML/tabby | Good to track for self-hosted completion/chat; less of a full autonomous coding agent than Cline/OpenCode/Codex. |
| **Sourcegraph Cody** | Code assistant | Active but strategically secondary | N/A | Commercial / mixed history | https://sourcegraph.com/cody | Historically important, but Sourcegraph’s current flagship agentic product is Amp. |

## Commercial / proprietary repo-centric coding agents and IDEs

| Tool | Category | Status | Company | Notes |
|---|---|---|---|---|
| **Claude Code** | Terminal / IDE / web / desktop coding agent | Active | Anthropic | Must be updated from “terminal-only.” Claude’s coding product now spans CLI, IDE integrations, web/cloud workflows, desktop sessions, code review, and security-oriented team features. |
| **Claude Cowork** | GUI work/coding-adjacent agent | Active | Anthropic | Related Claude agent surface for non-technical users and file/task workflows; not a normal code editor. |
| **Cursor** | AI IDE | Active | Anysphere | Proprietary AI-first code editor with agent workflows. |
| **Windsurf** | AI IDE | Active | Cognition / Windsurf | Proprietary agentic IDE with deep codebase context. |
| **Trae** | AI IDE | Active | ByteDance | Proprietary/free AI IDE. |
| **GitHub Copilot Coding Agent / Agent HQ** | IDE assistant + issue-to-PR agent | Active | GitHub / Microsoft | Should be updated beyond autocomplete/chat. Copilot now includes agent mode and agentic GitHub workflows. |
| **OpenAI Codex Web / App** | Cloud coding agent | Active | OpenAI | Commercial Codex product surface, separate from the open-source Codex CLI repo. |
| **Amp** | Terminal/editor coding agent | Active | Sourcegraph | Important 2026 omission. Add as high priority. |
| **Amazon Q Developer** | AI coding assistant | Active | AWS | Enterprise/AWS coding assistant. |
| **Kiro** | Agentic/spec-driven IDE | Active | AWS / Amazon | Important commercial IDE focused on spec-driven software development. |
| **Google Antigravity** | Agent-first IDE / agent manager | Active | Google | Replacement direction for Firebase Studio; agent-first IDE with manager/orchestration workflow. |
| **Augment Code** | Enterprise coding assistant | Active | Augment | Commercial assistant for large codebases. |
| **Tabnine** | AI coding assistant | Active | Tabnine | Privacy/enterprise-oriented commercial coding assistant. |
| **Jules** | Autonomous coding agent | Active | Google | Google async coding agent. |
| **Devin** | Autonomous software engineer | Active | Cognition | Commercial autonomous development platform. |
| **Factory AI** | Autonomous dev platform | Active | Factory | Commercial AI “Droids” for enterprise development workflows. |
| **CodeRabbit** | Code review agent | Active | CodeRabbit | Commercial AI code review platform. |
| **Qodo** | Code quality/testing | Active | Qodo | Commercial code quality/testing platform. |
| **Warp** | AI terminal | Active | Warp | Commercial AI terminal. |

## Commercial app builders / vibe-coding platforms

These are adjacent to agentic coding tools. They are often less repo-centric than Claude Code, Codex, Cursor, OpenCode, or Antigravity, but users compare them for “build me an app” workflows.

| Tool | Status | Company | Notes |
|---|---|---|---|
| **bolt.new** | Active | StackBlitz | Web app builder with browser-based coding environment. |
| **Lovable** | Active | Lovable | Popular natural-language full-stack app builder. |
| **Replit Agent** | Active | Replit | Cloud IDE + app generation + deployment workflow. |
| **v0** | Active | Vercel | UI/app generation, especially strong for React/Next.js interface work. |
| **Base44** | Active | Wix / Base44 | Important 2025-2026 vibe-coding/app-builder platform. |
| **Emergent** | Active | Emergent | Commercial AI app builder. |
| **Hostinger Horizons** | Active | Hostinger | No-code/AI web app creation platform. |
| **create.xyz** | Active | Create | Prompt-based app/site builder. |
| **Builder.io** | Active | Builder.io | Visual development and design-to-code tooling. |
| **GitHub Spark** | Active | GitHub | Natural-language app creation inside GitHub ecosystem. |

## Sunsetting, deprecated, renamed, or replaced

| Tool | Status | Replacement / current treatment | Notes |
|---|---|---|---|
| **Firebase Studio** | Sunsetting / deprecated | Google Antigravity and Google AI Studio | Keep for history, but remove from active recommended list. Final shutdown is planned for March 22, 2027. Core Firebase backend services continue separately. |
| **Project IDX** | Renamed / replaced | Firebase Studio, then sunset path to Antigravity / AI Studio | Project IDX became Firebase Studio; do not list IDX separately as an active product. |
| **app.build / appdotbuild-agent** | Not actively maintained | Research/reference only | Repo says it is not actively maintained and the managed service was discontinued. Latest visible commit: February 2, 2026. |
| **GitHub Copilot “Ghostwriter” wording** | Outdated naming | GitHub Copilot / Copilot Coding Agent | Use current GitHub Copilot naming and separate the older completion/chat feature set from the newer coding-agent workflows. |
| **OpenAI Codex as only a “model”** | Outdated framing | Codex CLI + Codex web/cloud product | The repo should distinguish the open-source CLI from OpenAI’s commercial Codex product surface. |
| **Claude Code as terminal-only** | Outdated framing | Claude Code product family | Keep the tool, but update description to include CLI, IDE, web/cloud, desktop sessions, review/security. |

## Highest-priority missing additions

1. **Amp** — too important to omit from a 2026 coding-agent list.
2. **OpenCode** — major open-source CLI/desktop coding agent.
3. **Kilo Code** — major open-source IDE/CLI platform.
4. **Goose** — strong open-source local agent with MCP/provider breadth.
5. **Google Antigravity** — important commercial agent-first IDE and Firebase Studio replacement direction.
6. **Kiro** — important commercial/spec-driven agentic IDE.
7. **Claude Cowork / Claude Code Review / Claude Code Security** — Claude should be represented beyond terminal-only Claude Code.
8. **Base44** and **Emergent** — important app-builder/vibe-coding comparables.
9. **GitHub Spark** — important GitHub-native app builder to track separately from Copilot.

## README cleanup recommendation

The README should not say the repo is an “open-source catalog” of tools, because the catalog contains many proprietary tools. Better wording:

> A catalog of agentic coding tools, AI IDEs, coding agents, and app builders, clearly separated by open-source, source-available, commercial, and deprecated status.

The main README should include these top-level groups:

1. Open-source / self-hostable
2. Source-available / mixed
3. Commercial coding agents and IDEs
4. Commercial app builders / vibe-coding platforms
5. Sunsetting / deprecated / renamed

This makes the catalog much more trustworthy than one giant mixed list.
