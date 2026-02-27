# AI Agents -- Apple Platform Engineering Skills 🚀

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-1.2.1-green.svg) ![Open
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

Skills are installable into compatible AI tooling using the `skills`
CLI.

------------------------------------------------------------------------

## 📂 Repository Structure

    skills/
      apple-accessibility-advisor/
        SKILL.md
        accessibility-patterns.md
        swiftui-examples.md
        testing-strategies.md
        wcag-guidelines.md
    .claude/
      manifest.json

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
npx skills add saurabhdave/aiagents --skill apple-accessibility-advisor
```

------------------------------------------------------------------------

## 🤖 Claude Code Integration

This repository supports Claude Code skill loading.

If using Claude Code:

1.  Clone this repository.
2.  Ensure `.claude/manifest.json` exists.
3.  Run:

``` bash
claude skills add saurabhdave/aiagents --skill apple-accessibility-advisor
```

Claude will automatically apply the Output Contract defined in
`SKILL.md`.

------------------------------------------------------------------------

## 📈 Roadmap

-   SwiftUI Performance Advisor
-   iOS Architecture Reviewer
-   Accessibility Testing & CI Automation
-   UIKit to SwiftUI Migration Assistant
-   Concurrency & Async/Await Modernization Advisor

------------------------------------------------------------------------

## 📄 License

MIT © 2026 Saurabh Dave

Maintained by Saurabh Dave.
