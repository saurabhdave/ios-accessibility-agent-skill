# AGENTS Integration Guide

This file provides machine‑friendly context and invocation examples to help AI agents
(e.g. Copilot, Claude, Cursor, or custom agent runtimes) use the skills in this
repository effectively.

## Purpose

Enable programmatic discovery, safe invocation, and predictable outputs from the
`apple-accessibility-advisor` skill and any future skills in this repo.

## Skill Metadata (machine‑readable)

- `skill_id`: `apple-accessibility-advisor`
- `version`: `1.0.0`
- `author`: `Saurabh Dave`
- `platforms`: ["iOS","iPadOS","macOS","watchOS","visionOS","tvOS"]
- `areas`: ["accessibility","swiftui","uikit","appkit","testing"]
- `manifest_file`: `skills/apple-accessibility-advisor/SKILL.md`

Agents may parse `SKILL.md` for prompt templates, examples, and response structure.

## Expected Response Structure

When asked to review or suggest changes, the skill should return a response with
these labelled sections (plain text or structured JSON):

1. Issues Identified — concise list of problems.
2. Recommended Improvements — prioritized actionable fixes.
3. Code Examples — minimal, copyable Swift/SwiftUI snippets when applicable.
4. Testing Strategy — how to validate the change (manual + automation).
5. Production Considerations — performance, localization, and audit notes.

Agents should prefer this structured output when generating replies.

## Invocation Examples (system/prompt)

- Short review:
  "Review this SwiftUI `ProfileRow` for accessibility issues and return the
  structured response with issues, fixes, code and tests."

- Deep audit:
  "Run an accessibility audit checklist for this module and produce a prioritized
  remediation plan suitable for inclusion in a sprint."

- Platform specific:
  "Explain how to adapt this VoiceOver behavior for watchOS and tvOS, include
  code and testing notes."

## Parsing Guidance for Agents

- Prefer the `SKILL.md` for metadata and the docs folder for patterns/examples.
- If extracting code examples, return only fenced code blocks marked `swift`.
- Validate that any returned code follows platform constraints mentioned in the
  skill (e.g. WatchKit or tvOS differences).

## Safety / Constraints

- Do not modify user files automatically without an explicit confirmation step.
- When suggesting accessibility labels or copy, mark any assumed/localized text
  clearly so the human reviewer can verify translations.

## Testing Prompts (use in CI or regression)

- "Given the `ProfileRow` code, does every interactive view have an
  accessibilityLabel and hint? Return `true` or a list of missing elements."
- "Check this README and SKILL.md for required sections; return `ok` or a list
  of missing headings."

## Maintenance

- Update this `AGENTS.md` whenever new skills are added or the `SKILL.md` format
  changes.

---

File location: `AGENTS.md` — place this alongside `README.md` for agent discovery.