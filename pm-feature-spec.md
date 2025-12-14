# Visual Feature Spec: Fix Header Truncation on Android Screens

## Feature Name
Android Header Safe-Area Fix

---

## Problem Statement
On several Android screens (Home, Overview, Focus, Stats), the top header content is partially hidden behind the system status bar. Text and icons appear truncated, which reduces readability and creates uncertainty for users about whether the screen is loading correctly or broken.

This issue is especially noticeable during onboarding and early usage, where visual clarity is critical for building trust.

---

## User Story
As a Focus Bear user,  
I want all headers and key information to be fully visible on screen,  
so I can understand the interface clearly without distraction or confusion.

---

## Visual Reference (Description)

Current State:

Header text overlaps with Android system status bar.

Top padding is insufficient.

Important information appears clipped.

Proposed State:

Safe-area padding applied correctly.

Header text fully visible below system status bar.

Consistent spacing across all primary screens.

---


## Acceptance Criteria

### Functional
- Headers must not overlap with the Android system status bar.
- All header text and icons must be fully visible on all supported screen sizes.
- The fix must apply consistently across:
  - Home
  - Overview
  - Focus
  - Stats

### UX & Accessibility
- Visual spacing should feel consistent and uncluttered.
- No loss of content hierarchy due to padding changes.
- Text remains readable at standard font sizes.

### Technical
- Proper use of Android safe-area or insets.
- No layout regressions introduced on iOS.
- No additional scrolling required due to padding changes.

### Definition of Done
- Headers are fully visible on Android devices.
- Tested on at least two different Android screen sizes.
- No new UI overlap issues introduced.
- QA sign-off completed.

---

## Reflection

### How Visual Elements Improve the Spec
Even simple annotated screenshots or text-based wireframes make the issue immediately clear. Developers can see exactly what is wrong and what “fixed” should look like without guessing.

### What Was Challenging
The hardest part was keeping the spec small and focused. It’s easy to expand into broader layout refactors, but this task required isolating one clear, testable improvement.

### How This Process Could Be Improved
Having a lightweight template for small visual fixes would speed things up. Including before/after screenshots directly in GitHub issues would also reduce back-and-forth during implementation.

---

