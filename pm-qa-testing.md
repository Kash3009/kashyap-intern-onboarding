
## PM Involvement in QA & User Testing

## Role of a PM in QA and Testing
A Product Manager plays a critical role in quality assurance by acting as the final advocate for the user. While QA testers focus on identifying bugs and edge cases, PMs ensure that the feature behaves as intended, aligns with the original requirements, and delivers the expected user experience.

PMs are responsible for:
- Validating features against the original spec and acceptance criteria
- Identifying UX inconsistencies or unexpected behaviours
- Ensuring edge cases are considered
- Deciding whether a feature is ready for release or needs iteration

---

## How QA Teams Test Features
QA teams typically:
- Write test cases based on acceptance criteria
- Test happy paths and edge cases
- Verify behaviour across devices and environments
- Log bugs with clear steps to reproduce
- Re-test after fixes are applied

Their focus is correctness and stability, while PMs focus on *intent* and *experience*.

---

## Why PM Testing Matters
PM testing catches issues that automated tests and QA scripts may miss, such as:
- Confusing copy or unclear interactions
- Flows that technically work but feel unintuitive
- Inconsistencies between the spec and implementation
- Small UX details that affect trust and usability

PM involvement ensures features don’t just work — they work *well* for users.

---

## Task: Feature Testing Observation

### Feature Tested
Focus session timer setup flow (onboarding / early usage)

*(Note: This test was conducted on the live app due to limited access to unreleased features.)*

---

## Comparison: Spec vs Implementation

### What the Spec Intended
- Clear and predictable timer interaction
- Smooth scrolling behaviour
- No visual overlap with system UI
- Clear formatting of time values

### What Was Observed
- Timer scroll animation feels static and stops mid-motion
- Time formatting includes unclear elements (e.g., “55..”)
- Header content overlaps with the Android system status bar on some screens
- UX issues persist even when Super Strict Mode is enabled

---

## Identified Issue
The timer setup flow technically functions, but does not fully align with UX expectations defined in earlier feature discussions. The interaction lacks clarity and predictability, which may increase cognitive load for neurodivergent users.

---

## Reflection

### Difference Between Spec and Implementation
The implementation meets functional requirements but falls short on UX polish. Visual clarity, spacing, and animation behaviour differ from what a smooth onboarding experience would ideally provide.

### One Improvement to the Testing Process
PMs should be involved earlier in QA, not just after development is complete. A short UX review before final QA sign-off could catch issues related to layout, spacing, and interaction flow sooner.

### How PMs Can Reduce Production Issues
- Write clear, testable acceptance criteria
- Review features alongside QA, not after
- Test flows from a first-time user perspective
- Encourage early feedback loops with designers and engineers

---

## Summary
PM involvement in QA ensures that features deliver not only correct behaviour, but also the intended user experience. At Focus Bear, where clarity and emotional safety matter deeply, PM-led testing is essential for maintaining trust and usability.
