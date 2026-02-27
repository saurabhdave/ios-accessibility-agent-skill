# AI Agents -- Apple Platform Engineering Skills 🚀

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-1.2.3-green.svg) ![Open
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


## What Makes This Skill Different

**Enterprise-oriented.**\
Designed for production applications --- not tutorial-level examples.

**Architectural focus.**\
Prioritizes scalable, multi-platform accessibility patterns.

**Deterministic output.**\
Enforces a strict Output Contract to ensure consistent structured
responses.

**Agent-framework agnostic.**\
Works with Claude Code, Cursor, Copilot-style agents, and other tools
supporting the Agent Skills format.

------------------------------------------------------------------------

## Skill Structure

    aiagents/
    ├── .claude/
    │   └── manifest.json
    ├── skills/
    │   └── apple-accessibility-advisor/
    │       ├── SKILL.md
    │       ├── accessibility-patterns.md
    │       ├── swiftui-examples.md
    │       ├── testing-strategies.md
    │       └── wcag-guidelines.md
    ├── AGENTS.md
    ├── CHANGELOG.md
    ├── LICENSE
    └── README.md

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

## How to Use This Skill

### Option A --- Using skills.sh (Recommended)

``` bash
npx skills add saurabhdave/aiagents --skill apple-accessibility-advisor
```

Visit https://skills.sh to learn more about the Agent Skills format.

------------------------------------------------------------------------

### Option B --- Claude Code Plugin

#### Personal Usage

    /plugin marketplace add saurabhdave/aiagents
    /plugin install apple-accessibility-advisor@aiagents

#### Project Configuration (Team-Wide)

Add this to `.claude/settings.json`:

``` json
{
  "enabledPlugins": {
    "apple-accessibility-advisor@aiagents": true
  },
  "extraKnownMarketplaces": {
    "aiagents": {
      "source": {
        "source": "github",
        "repo": "saurabhdave/aiagents"
      }
    }
  }
}
```

Committing this file enables the skill automatically for all team
members.

------------------------------------------------------------------------

### Option C --- Manual Installation

1.  Clone the repository:

``` bash
git clone https://github.com/saurabhdave/aiagents.git
```

2.  Copy or symlink: `skills/apple-accessibility-advisor/` into your AI tool's skills directory.

3.  Restart or reload your agent.

Refer to your tool documentation for skills directory location:

-   Claude Code
-   Cursor
-   Windsurf
-   Other Agent-Skills compatible tools

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
