# AI Agents -- Apple Platform Engineering Skills 🚀

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-1.2.0-green.svg) ![Open
Agent
Skills](https://img.shields.io/badge/OpenAgentSkills-compatible-purple)

------------------------------------------------------------------------

## About

This repository provides Open Agent Skills for Apple platform
engineering tasks.

Each skill encapsulates production-grade domain expertise and is
designed to be consumed by compatible AI agents using the Open Agent
Skills specification via `npx skills`.

Audience: Intermediate to senior Apple platform engineers.\
Focus: Accessibility, architecture, performance, and enterprise
readiness.

------------------------------------------------------------------------

## Overview

A structured collection of reusable AI skills that help Apple platform
developers:

-   Audit and improve accessibility
-   Architect scalable systems
-   Optimize performance
-   Enforce platform best practices
-   Prepare for enterprise review and compliance

Skills are installable into compatible AI tooling (Claude Code, Cursor,
Copilot extensions, etc.) using the `skills` CLI.

------------------------------------------------------------------------

## 📂 Repository Structure

    skills/
      apple-accessibility-advisor/
        SKILL.md
        accessibility-patterns.md
        swiftui-examples.md
        testing-strategies.md
        wcag-guidelines.md

Each skill folder contains:

-   `SKILL.md` → Agent instructions and output contract
-   Supporting modules → Implementation patterns and reference guidance

------------------------------------------------------------------------

## 🧰 Current Skills

  ------------------------------------------------------------------------------
  Skill                           Description
  ------------------------------- ----------------------------------------------
  `apple-accessibility-advisor`   Production-grade accessibility audit and
                                  implementation advisor for Apple platform
                                  applications (iOS, iPadOS, macOS, watchOS,
                                  visionOS, tvOS).

  ------------------------------------------------------------------------------

------------------------------------------------------------------------

## 📦 Installation

``` bash
# Install the Apple Accessibility Advisor
npx skills add saurabhdave/aiagents --skill apple-accessibility-advisor
```

After installation, invoke the skill in your AI agent with prompts such
as:

-   "Audit this SwiftUI view for accessibility compliance."
-   "Make this UIKit screen VoiceOver compliant."
-   "Validate this feature against WCAG 2.1 AA."
-   "Design a multi-platform accessibility strategy."

See `skills/apple-accessibility-advisor/SKILL.md` for full usage
guidance.

------------------------------------------------------------------------

## 📈 Roadmap

Planned additions:

-   SwiftUI Performance Advisor
-   iOS Architecture Reviewer
-   Accessibility Testing & CI Automation
-   UIKit to SwiftUI Migration Assistant
-   Concurrency & Async/Await Modernization Advisor

Suggestions are welcome --- open an issue to propose a new skill.

------------------------------------------------------------------------

## 🤝 Contributing

To contribute:

1.  Fork the repository.
2.  Create a new branch.
3.  Add a new folder under `skills/` with your `SKILL.md` and supporting
    modules.
4.  Update the skills table in this README.
5.  Ensure Markdown formatting is clean.
6.  Submit a pull request with a clear description of the skill.

See [`CONTRIBUTING.md`](./CONTRIBUTING.md) for full guidelines.

------------------------------------------------------------------------

## 📄 License

MIT © 2026 Saurabh Dave

------------------------------------------------------------------------

Maintained by Saurabh Dave.
