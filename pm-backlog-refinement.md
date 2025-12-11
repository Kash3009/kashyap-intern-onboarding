
## Backlog Item Refinement  
Improving Onboarding Greeting & Personalisation

---

## Problem Statement
The onboarding currently displays the user’s email address as the greeting (e.g., "Hi kashyap01…") before collecting their preferred name.  
This creates an impersonal first impression and breaks the tone of warmth and safety expected for neurodivergent users.  
Emojis used on the screen feel generic and off-brand for Focus Bear.

---

## User Story
As a new Focus Bear user,  
I want the app to ask for my preferred name before greeting me,  
so the onboarding feels personal, friendly, and aligned with the product’s supportive mission.

---

## Acceptance Criteria

### Required Behaviour
- The first onboarding screen **must not** show the user’s email.  
- The first screen asks: “What should we call you?”  
- A text input captures the preferred name.  
- After submitting, the next screen greets the user with:  
  “Hi <Name> 👋 Ready to build better habits?”  
- The name persists in the user's profile for future app sessions.

### Input Validation
- Empty submission is not allowed; show: “Please enter a name.”  
- Standard characters only (letters, numbers, basic punctuation).  
- If saving the name fails, the app displays a retry message.

### UX & Visual Requirements
- Replace generic emojis with a Focus Bear character illustration.  
- Design must follow existing spacing/typography standards.  
- All text must meet accessibility contrast requirements.  
- Status bar (time, battery, notifications) must remain visible.

### Edge Cases
- If a name already exists in stored profile → skip the name entry step.  
- If onboarding is interrupted mid-flow, the app resumes at the correct step.

### Definition of Done
- All acceptance criteria met.  
- Behaviour confirmed on Android and iOS.  
- No console/log errors related to onboarding or saving name.  
- Screenshots of implemented UI included in the PR.  
- QA signs off after testing input validation, flow logic, and visual updates.

---

## Technical Notes
- Add/confirm presence of `preferred_name` in user profile schema.  
- Update onboarding sequence (name collection → personalised greeting → next steps).  
- Ensure syncing logic for the new field aligns with backend conventions.  
- Minor UI update required: text field, mascot illustration, CTA button layout.

---

## Reflection

### Missing Details in Original Item
The original backlog item lacked a clear problem statement, no user story, no acceptance criteria, and no edge cases. Developers would have had to guess the intended behaviour.

### Why Refinement Helps Developers
Clear acceptance criteria remove ambiguity, reduce rework, and allow engineers to implement confidently. It also supports consistent UX and makes QA testing straightforward.

### Challenges Writing Acceptance Criteria
Balancing clarity with flexibility was the hardest part. I had to consider user experience, accessibility needs, emotional tone, and technical feasibility — all core parts of PM decision-making at Focus Bear.

