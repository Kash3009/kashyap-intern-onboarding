# Feature One-Pager: Focus Session Experience (Timer, Distraction Blocking & Music)

## Feature Name
Focus Session Experience – Timer, Distraction Blocking & Focus Music

---

## Problem Statement

The Focus feature is the core of the Focus Bear app, but during first-time and early usage, users may feel uncertain about what will happen once they start a focus session.  

Key areas of friction include:
- Unclear expectations around distraction blocking before starting
- Visual and spacing issues that reduce confidence
- Timer selector behaviour that feels inconsistent
- Cognitive overload for neurodivergent users at the moment of starting focus

For users with ADHD or low attention span, predictability and clarity are essential. Any hesitation at this stage risks users abandoning or delaying focus sessions, reducing early engagement and habit formation.

---

## Target Users

- Users with ADHD or low attention span
- Neurodivergent users who benefit from structured, predictable workflows
- First-time users starting their first focus session
- Existing users who rely on distraction blocking and focus music for deep work

---

## User Stories & Scenarios

### User Stories
- As a user with ADHD, I want to clearly understand what will be blocked before I start focusing so I can commit without anxiety.
- As a new user, I want starting a focus session to feel simple and reassuring so I don’t overthink or delay starting.
- As a user trying to avoid distractions, I want clear feedback when I open distracting apps so I can consciously decide whether it’s worth breaking focus.
- As a user, I want supportive focus music options so I can enter a focused mental state more easily.

### Scenarios
- User opens the app → navigates to the Focus tab
- User selects a task, duration, and focus music
- App explains (briefly) what distraction blocking will do
- User starts focus session
- User attempts to open a distracting app → reflective prompt appears
- Focus session completes → user reviews stats and progress

---

## Wireframe / Annotated User Journey (Annotated Visual Flow)

Below is a step-by-step annotated representation of the user journey, referencing specific screen elements and layout zones to act as a visual guide for developers and designers.

### Screen 1: Focus Tab (Setup)
**Elements:**
- Task input field
- Timer selector
- Focus music selection (e.g. ADHD Blocked, Brain Energiser)

**Current issues:**
- Timer scroll behaviour feels abrupt
- Numeric formatting is unclear (e.g. “55..”)

**Proposed changes:**
- Smooth, infinite looping timer scroll (native picker behaviour)
- Clear time labels (e.g. “55 min”)


Image: <img width="325" height="728" alt="image" src="https://github.com/user-attachments/assets/9bf70bf5-8db4-4d71-b2b0-7a340dceef37" />

---

### Screen 2: Start Focus Confirmation
**Elements:**
- “Start Focus” CTA
- Distraction blocking toggle

**Current issues:**
- Users are not fully prepared for what blocking will do

**Proposed changes:**
- Short preview text explaining:
  - Which apps will be blocked
  - What happens if the user tries to open them


Image: <img width="323" height="731" alt="image" src="https://github.com/user-attachments/assets/617f7845-50da-459d-9e84-0d0663495118" />

---

### Screen 3: Active Focus Session
**Elements:**
- Timer countdown
- Music playing
- Super Strict Mode indicator (if enabled)

**Current issues:**
- Layout issues persist across modes

**Proposed changes:**
- Apply consistent spacing and layout rules globally


Image 1 : <img width="327" height="726" alt="image" src="https://github.com/user-attachments/assets/7d6184f0-22ca-4c08-8b73-dcee3c9c13d0" />
Image 2: <img width="341" height="757" alt="image" src="https://github.com/user-attachments/assets/71b035f5-a440-429c-8f71-ebc1bf3a4c40" />

---

### Screen 4: Distraction Interruption Prompt
**Elements:**
- App name (e.g. Instagram, YouTube)
- Reflective question (“Why do you want to use this?”)
- Options to continue or return to focus

**Value:**
- Encourages intentional decision-making instead of mindless distraction


Image: <img width="323" height="731" alt="image" src="https://github.com/user-attachments/assets/67105dc3-69e4-4e80-a334-db1ac5b9db25" />

---

### Screen 5: Stats / Review
**Elements:**
- Focus duration
- App usage insights

**Proposed changes:**
- Clear hierarchy and spacing to reduce cognitive load

App and Health Stats Image: <img width="342" height="757" alt="image" src="https://github.com/user-attachments/assets/6335b40e-bbdb-4425-b04e-3883d07487fc" />

---

**Summary Flow:**  
Focus Tab → Setup → Start Focus → Active Focus Session → Distraction Prompt (if triggered) → Stats Review

---

## Acceptance Criteria

- Focus session setup is visually clear with no clipped headers or truncated elements
- Timer selector scrolls smoothly and displays clean, readable time values
- Users understand what distraction blocking does *before* starting a session
- Distraction prompts clearly explain why the app is blocked and encourage reflection
- Focus music options are visible and easy to select without overwhelming the user

---

## Open Questions

- Should experienced users be able to skip the distraction-blocking explanation after their first few sessions?
- How much explanation is “just enough” before starting focus without increasing cognitive load?
- Should focus music preferences persist automatically between sessions?

---

## Reflection

### Hardest Part of Writing This One-Pager
Balancing clarity with simplicity—explaining how distraction blocking works without overwhelming users right before they start focusing.

### How I Would Present This to Developers & Designers
I’d walk through the visual flow step by step, explain where users hesitate, and highlight how small UX improvements can significantly increase focus session starts and completion rates.
