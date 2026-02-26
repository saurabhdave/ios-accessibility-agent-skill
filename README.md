# AI Agents – Apple Platform Engineering Skills 🚀

## About

This repository houses a set of AI‑driven skills tailored for Apple platform engineers.
Each skill encapsulates domain expertise—from accessibility audits to performance
optimizations—and is intended to be consumed by AI agents (via `npx skills`) in chat,
code review, or automated workflows. The goal is to provide on‑demand, standardized
recommendations that promote best practices across teams.

## Overview

A growing collection of **reusable AI agent skills** that help Apple platform developers
build better‑architected, high‑performance, and accessible apps. Skills are delivered as
npm modules and can be plugged into your AI‑powered tooling via `npx skills`.


---

## 🧰 Current Skill(s)

| Skill | Description |
|-------|-------------|
| `apple-accessibility-advisor` | Enterprise‑grade accessibility guidance for SwiftUI, UIKit, AppKit, WatchKit, and platform-specific APIs across iOS, iPadOS, macOS, watchOS, visionOS, and tvOS. |


### Installation

```bash
# install a specific skill
npx skills add saurabhdave/aiagents --skill apple-accessibility-advisor
```

> Once added, invoke the skill by asking your AI agent to review code, recommend
> improvements, or explain accessibility concepts – see `skills/apple-accessibility-advisor/SKILL.md`
> for sample prompts.


---

## 📈 Roadmap

More skills are planned and the project will remain open to contributions:

- SwiftUI Performance Advisor
- iOS Architecture Reviewer
- Accessibility Testing & CI Automation
- UIKit to SwiftUI Migration Assistant

Feel free to open an issue if you have a new skill idea!


---

## 🤝 Contributing

We welcome contributions from the community. To get started:

1. Fork the repo and create a new branch for your feature/skill.
2. Add a new folder under `skills/` with your `SKILL.md` and any supporting docs or example code.
3. Update the root `README.md` table and the `skills` npm packaging script if needed.
4. Run `markdownlint` and ensure any Swift snippets compile (we use GitHub Actions to verify later).
5. Submit a pull request and describe the skill's purpose and usage.

See [`CONTRIBUTING.md`](./CONTRIBUTING.md) for more details.


---

## 📄 License

MIT © 2026 Saurabh Dave


---

*This repository is maintained by the AI platform engineering team. Happy building!*