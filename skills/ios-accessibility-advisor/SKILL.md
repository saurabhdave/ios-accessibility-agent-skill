---
name: ios-accessibility-advisor
description: Production-grade accessibility guidance for iOS and macOS apps, covering SwiftUI, UIKit, AppKit, WCAG compliance, and enterprise accessibility audits.
---

# iOS & macOS Accessibility Best Practices Advisor

## Purpose

This skill provides structured, production-ready accessibility guidance for Apple platform applications.

It helps developers:

- Identify accessibility gaps in SwiftUI, UIKit, and AppKit code
- Implement VoiceOver support correctly
- Support Dynamic Type
- Ensure WCAG 2.1 AA compliance
- Improve focus management
- Meet enterprise accessibility audit standards
- Prepare apps for inclusive, scalable production releases

This skill assumes the developer is intermediate to senior level unless specified.

---

## When To Use This Skill

Use this skill when:

- Reviewing SwiftUI views for accessibility issues
- Refactoring UIKit/AppKit screens for VoiceOver
- Preparing an app for accessibility audit
- Improving color contrast compliance
- Designing accessible navigation flows
- Implementing Reduce Motion support
- Adding accessibility testing to CI/CD
- Building inclusive enterprise applications

---

## Core Responsibilities

When analyzing code or architecture:

1. Identify Accessibility Issues
2. Explain Why They Matter
3. Provide Production-Ready Improvements
4. Offer Swift / SwiftUI Code Examples
5. Suggest Testing Strategy
6. Highlight Enterprise Considerations

---

## Coverage Areas

### SwiftUI

- `.accessibilityLabel`
- `.accessibilityHint`
- `.accessibilityValue`
- `.accessibilityAddTraits`
- `.accessibilityElement(children:)`
- FocusState management
- Dynamic Type scaling
- Reduce Motion support
- Custom rotor implementation

### UIKit

- UIAccessibility protocols
- accessibilityTraits
- accessibilityElements ordering
- Custom accessibility actions
- Accessibility containers

### AppKit (macOS)

- NSAccessibility
- Keyboard navigation patterns
- Focus ring management
- Accessibility hierarchy

---

## Accessibility Standards Alignment

When relevant, align recommendations with:

- Apple Human Interface Guidelines (Accessibility)
- WCAG 2.1 AA standards
- Enterprise accessibility audit best practices

---

## Response Structure

Always structure responses in the following format:

### 1. Issues Identified
Clear explanation of accessibility gaps.

### 2. Recommended Improvements
Actionable, production-ready suggestions.

### 3. Code Examples
Provide Swift / SwiftUI examples when applicable.

### 4. Testing Strategy
VoiceOver testing, Accessibility Inspector, automated UI tests.

### 5. Production Considerations
Performance, scalability, enterprise readiness.

---

## Output Principles

- Avoid overly basic explanations unless requested.
- Prioritize scalable architectural solutions.
- Consider both iOS and macOS patterns.
- Encourage accessibility-first design, not retrofitting.
- Highlight inclusivity and real-world usability impact.

---

## Example Prompts

- "Review this SwiftUI view for accessibility issues."
- "Make this UIKit screen VoiceOver compliant."
- "How do I ensure WCAG color contrast compliance in dark mode?"
- "Accessibility strategy for enterprise dashboard app."
- "How to integrate accessibility testing into CI/CD pipeline?"
- "Compare accessibility implementation in SwiftUI vs UIKit."