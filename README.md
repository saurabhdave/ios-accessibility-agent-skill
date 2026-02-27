# AI Agents -- Apple Platform Engineering Skills 🚀

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-1.0.0-green.svg) ![Open
Agent
Skills](https://img.shields.io/badge/OpenAgentSkills-compatible-purple)

------------------------------------------------------------------------

## About

This repository contains reusable AI agent skills tailored for Apple
platform engineers.

Each skill encapsulates production-grade domain expertise --- from
accessibility audits to performance optimization --- and is designed to
be consumed by compatible AI agents using the Open Agent Skills
specification via `npx skills`.

The goal is to provide standardized, high-quality engineering guidance
that promotes best practices across teams.

------------------------------------------------------------------------

## Overview

A growing collection of structured AI skills that help Apple platform
developers build:

-   Accessible applications
-   Scalable architectures
-   High-performance UI
-   Enterprise-ready codebases

Skills can be installed into compatible AI tooling (Claude Code, Cursor,
Copilot extensions, etc.) using the `skills` CLI.

------------------------------------------------------------------------

## 📂 Repository Structure

    skills/
      apple-accessibility-advisor/
        SKILL.md
        accessibility-patterns.md      # consolidated patterns + examples
        swiftui-examples.md           # copy‑paste ready SwiftUI snippets
        testing-strategies.md
        wcag-guidelines.md

Each skill lives inside its own folder under `skills/` and contains:

-   `SKILL.md` → Skill definition and response structure
-   Supporting knowledge modules → Deep implementation guidance

------------------------------------------------------------------------

## 🧰 Current Skill(s)

  ------------------------------------------------------------------------------
  Skill                           Description
  ------------------------------- ----------------------------------------------
  `apple-accessibility-advisor`   Enterprise-grade accessibility guidance for
                                  SwiftUI, UIKit, AppKit, WatchKit, and
                                  platform-specific APIs across iOS, iPadOS,
                                  macOS, watchOS, visionOS, and tvOS.

  ------------------------------------------------------------------------------

------------------------------------------------------------------------

## 📦 Installation

``` bash
# Install the Apple Accessibility Advisor
npx skills add saurabhdave/aiagents --skill apple-accessibility-advisor
```

Once installed, invoke the skill in your AI agent by asking it to:

-   Review code for accessibility issues
-   Suggest VoiceOver improvements
-   Validate WCAG compliance
-   Recommend production-ready accessibility architecture

See `skills/apple-accessibility-advisor/SKILL.md` for example prompts.

------------------------------------------------------------------------

## 📈 Roadmap

More skills are planned. Contributions are welcome.

Planned additions:

-   SwiftUI Performance Advisor
-   iOS Architecture Reviewer
-   Accessibility Testing & CI Automation
-   UIKit to SwiftUI Migration Assistant
-   Concurrency & Async/Await Modernization Advisor

Open an issue if you have a new skill idea.

------------------------------------------------------------------------

## 🤝 Contributing

We welcome contributions from the community.

To contribute:

1.  Fork the repository.
2.  Create a new branch for your feature or skill.
3.  Add a new folder under `skills/` with your `SKILL.md` and supporting
    documentation.
4.  Update the skills table in this `README.md`.
5.  Ensure Markdown formatting is clean.
6.  Submit a pull request describing the skill's purpose and usage.

See [`CONTRIBUTING.md`](./CONTRIBUTING.md) for detailed guidelines.

------------------------------------------------------------------------

## 📄 License

MIT © 2026 Saurabh Dave

------------------------------------------------------------------------

Maintained by Saurabh Dave.
