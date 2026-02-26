# Accessibility Architecture Patterns

iOS & macOS Production Accessibility Guidance

This document defines reusable accessibility implementation patterns for
SwiftUI, UIKit, and AppKit applications.

These patterns are intended for production-grade, scalable applications
and enterprise audit readiness.

------------------------------------------------------------------------

# 1. VoiceOver Interaction Patterns

## Pattern: Explicit Labeling

### Problem

UI elements rely on visible text but lack semantic accessibility labels.

### Recommended Implementation (SwiftUI)

``` swift
Image(systemName: "trash")
    .accessibilityLabel("Delete item")
    .accessibilityHint("Removes this item permanently")
```

### UIKit

``` swift
deleteButton.accessibilityLabel = "Delete item"
deleteButton.accessibilityHint = "Removes this item permanently"
```

### Production Consideration

Never rely on icon-only meaning. Always provide semantic clarity.

------------------------------------------------------------------------

# 2. Focus Management Patterns

## Pattern: Logical Reading Order

### SwiftUI Solution

``` swift
VStack {
    header
    content
    footer
}
.accessibilityElement(children: .contain)
```

### UIKit Solution

``` swift
view.accessibilityElements = [headerView, contentView, footerView]
```

### Production Consideration

Validate with real VoiceOver testing, not just simulator preview.

------------------------------------------------------------------------

# 3. Dynamic Type Scalability Pattern

### SwiftUI Production Pattern

``` swift
Text("Profile")
    .font(.title)
    .minimumScaleFactor(0.8)
```

### UIKit Production Pattern

``` swift
label.font = UIFont.preferredFont(forTextStyle: .body)
label.adjustsFontForContentSizeCategory = true
```

### Production Consideration

Test at Accessibility Extra Extra Extra Large sizes.

------------------------------------------------------------------------

# 4. Color Contrast Compliance Pattern

## WCAG 2.1 AA Minimum Contrast

-   Normal text: 4.5:1
-   Large text: 3:1

### Recommended Practice

-   Validate with Accessibility Inspector
-   Avoid color-only indicators (add icon/text redundancy)

------------------------------------------------------------------------

# 5. Reduce Motion Pattern

### SwiftUI Implementation

``` swift
@Environment(\.accessibilityReduceMotion) var reduceMotion

if reduceMotion {
    showDetails = true
} else {
    withAnimation {
        showDetails = true
    }
}
```

### Production Consideration

Respect system-wide Reduce Motion preference.

------------------------------------------------------------------------

# 6. Custom Accessibility Actions Pattern

### SwiftUI Example

``` swift
.accessibilityAction(named: "Mark as Favorite") {
    markFavorite()
}
```

### UIKit Example

``` swift
let action = UIAccessibilityCustomAction(
    name: "Mark as Favorite",
    target: self,
    selector: #selector(markFavorite)
)
view.accessibilityCustomActions = [action]
```

------------------------------------------------------------------------

# 7. Accessibility Grouping Pattern

``` swift
.accessibilityElement(children: .combine)
```

------------------------------------------------------------------------

# 8. Enterprise Accessibility Audit Checklist

Before release, verify:

-   All interactive elements have labels
-   No contrast violations in light/dark mode
-   Dynamic Type does not break layout
-   VoiceOver navigation order matches UX
-   Custom gestures have accessible alternatives
-   Reduce Motion respected
-   Localization does not truncate accessible text

------------------------------------------------------------------------

# Architectural Principle

Accessibility must be integrated at: - Design phase - Component library
level - CI validation stage - Code review stage

Accessibility is not a feature --- it's architecture.
