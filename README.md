

# Agentic Coding Tools Catalog

A catalog of agentic coding tools, AI IDEs, coding agents, code review agents, and AI app builders, clearly separated by **open-source**, **source-available / mixed**, **commercial / proprietary**, and **sunsetting / deprecated** status.

## 🎯 Purpose

This repository tracks the fast-changing agentic coding ecosystem so developers can compare tools by capability, openness, product status, and best use case.

The catalog intentionally separates:

- open-source / self-hostable coding agents
- source-available or mixed-license projects
- commercial coding agents and AI IDEs
- commercial app builders / vibe-coding platforms
- deprecated, renamed, or sunsetting products

## 🔎 2026 status refresh

See the new comparison page:

- [`comparisons/open-source-vs-commercial-2026.md`](comparisons/open-source-vs-commercial-2026.md)

That page includes the latest cleanup notes, including:

- **Firebase Studio** should be treated as **sunsetting / deprecated**, not an active recommended platform.
- **Project IDX** should be treated as the older name for Firebase Studio, not a separate active product.
- **Claude Code** should no longer be described as terminal-only. Track it as a Claude coding product family spanning CLI, IDE, web/cloud, desktop sessions, review/security, and related Anthropic coding surfaces.
- **GitHub Copilot** should be updated beyond autocomplete/chat to include agent mode, coding agent, and issue-to-PR workflows.
- **OpenAI Codex** should be split between the open-source **Codex CLI** and OpenAI’s commercial Codex web/app product.

## 📋 Main tool groups

### Open-source / self-hostable tools

- **Aider** - terminal AI pair programmer with strong git workflow
- **Cline** - open-source autonomous VS Code coding agent
- **Roo Code** - Cline-family autonomous coding agent
- **Kilo Code** - open-source agentic engineering platform across IDE, CLI, Slack, and cloud surfaces
- **OpenCode** - open-source terminal / desktop coding agent
- **OpenAI Codex CLI** - open-source CLI coding agent
- **Gemini CLI** - Google’s open-source terminal coding agent
- **Goose** - open-source local desktop / CLI / API agent
- **Continue** - open-source IDE assistant for VS Code and JetBrains
- **PearAI** - open-source AI code editor; stale, do not treat as a top current option unless activity resumes
- **bolt.diy** - open-source/local version of bolt-style app generation
- **Convex Chef** - open-source AI app builder with Convex backend primitives
- **Wave Terminal** - open-source terminal with graphical widgets and AI capabilities

### Source-available / mixed-license tools

- **Crush** - terminal coding agent from Charmbracelet; source-available rather than pure open source
- **Tabby** - self-hosted code assistant with open-source core and commercial options
- **Pythagora / GPT Pilot** - open-source lineage with commercial product packaging to track carefully
- **Sourcegraph Cody** - historically important, but Sourcegraph’s current flagship agent product is Amp

### Commercial coding agents and AI IDEs

- **Claude Code** - Anthropic coding agent family, not just a CLI
- **Claude Cowork** - Anthropic GUI/workflow agent surface related to Claude Code direction
- **Cursor** - AI-first code editor built on VS Code
- **Windsurf** - agentic AI IDE
- **Trae** - ByteDance AI IDE
- **GitHub Copilot Coding Agent / Agent HQ** - Copilot agent mode and issue-to-PR workflows
- **OpenAI Codex Web / App** - commercial Codex coding agent surface
- **Amp** - Sourcegraph terminal/editor coding agent
- **Amazon Q Developer** - AWS enterprise AI coding assistant
- **Kiro** - AWS/Amazon spec-driven agentic IDE
- **Google Antigravity** - Google agent-first IDE / agent manager
- **Augment Code** - commercial assistant for large codebases
- **Tabnine** - privacy/enterprise-oriented AI coding assistant
- **Jules** - Google async autonomous coding agent
- **Devin** - Cognition autonomous software engineer
- **Factory AI** - commercial autonomous development platform
- **CodeRabbit** - commercial AI code review platform
- **Qodo** - commercial code quality and testing platform
- **Warp** - commercial AI terminal

### Commercial app builders / vibe-coding platforms

- **bolt.new** - StackBlitz browser-based AI app builder
- **Lovable** - natural-language full-stack app builder
- **Replit Agent** - cloud IDE + app generation + deployment workflow
- **v0** - Vercel UI/app generation platform
- **Base44** - commercial AI app builder
- **Emergent** - commercial AI app builder
- **Hostinger Horizons** - no-code/AI web app creation platform
- **create.xyz** - prompt-based app/site builder
- **Builder.io** - visual development and design-to-code tooling
- **GitHub Spark** - GitHub-native natural-language app builder

### Sunsetting, deprecated, renamed, or replaced

- **Firebase Studio** - sunsetting / deprecated; keep for history, but remove from active recommended tools
- **Project IDX** - older name / predecessor of Firebase Studio
- **OpenAI Codex as only a “model”** - outdated framing; split into Codex CLI and Codex web/app product
- **Claude Code as terminal-only** - outdated framing; update to Claude coding product family
- **GitHub Copilot as autocomplete-only** - outdated framing; update to include agent mode and coding agent workflows

## 🗂️ Repository structure

```
/
├── README.md
├── tools/
│   ├── cursor.md
│   ├── windsurf.md
│   ├── github-copilot.md
│   └── [other-tools].md
├── comparisons/
│   ├── desktop-ides.md
│   ├── web-platforms.md
│   ├── open-source-tools.md
│   └── open-source-vs-commercial-2026.md
└── CONTRIBUTING.md
```

## Suggested next tool pages

High-priority missing pages to add next:

- `tools/amp.md`
- `tools/opencode.md`
- `tools/kilo-code.md`
- `tools/goose.md`
- `tools/crush.md`
- `tools/google-antigravity.md`
- `tools/kiro.md`
- `tools/base44.md`
- `tools/emergent.md`
- `tools/github-spark.md`

## 📊 Tool rating system

Each tool can be evaluated on:

- agentic capability
- repo/codebase awareness
- edit/run/test loop quality
- autonomy and safety controls
- model/provider flexibility
- IDE/CLI/cloud availability
- openness and self-hostability
- pricing and enterprise readiness

## 🏷️ License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

*Last updated: June 2026*
