## Goal
The goal of this task is to use PostHog analytics to understand how users behave inside Focus Bear, identify a meaningful drop-off point in the user journey, and suggest a data-driven improvement to reduce that drop-off.

---

## Research & Learn

### What key user metrics should PMs track in PostHog?
For a habit-building and focus product like Focus Bear, the most important metrics include:

- **Acquisition & Activation**
  - Sign-up completion rate
  - Onboarding completion
  - Time to first value (first routine completed or first focus session completed)

- **Engagement**
  - Daily Active Users (DAU)
  - Monthly Active Users (MAU)
  - Completion events such as:
    - `complete-morning-routine-activity`
    - `completed-focus-session`

- **Retention**
  - Return usage after first successful focus session
  - Stickiness (DAU / MAU ratio), especially for paid users

- **Friction & Drop-off**
  - Funnel drop-offs
  - App quit events
  - Error or interruption-related exits

---

### How do companies identify drop-off points in user journeys?
Drop-off points are usually identified by:
- Creating **funnels** (e.g. onboarding → first session → completed session)
- Comparing completion vs abandonment between steps
- Reviewing **quit or exit events** during critical flows
- Segmenting by platform, feature usage, or user type

In Focus Bear’s case, quit behaviour during focus usage is a strong indicator of friction.

---

### What role does analytics play in validating customer feedback?
Customer feedback explains *why users feel something is wrong*.  
Analytics confirms *how often it happens and where*.

When both align, it becomes a high-confidence signal for prioritisation.

---

## Data Reviewed in PostHog

I reviewed the following PostHog insights:

- **Daily Active Users (DAU)** – all-time trend
- **Monthly Active Users (MAU)** – broken down by platform and completion events
- **Quit Reasons** – breakdown of why users exit the app
- **Stickiness Ratio for Paid Users**

Screenshots were captured directly from PostHog for each of these views.

---

## Identified Drop-Off Point

### Drop-off: Users quitting during focus usage instead of completing focus sessions

**Evidence from PostHog (Quit Reasons):**
The most frequent quit reasons include:
- *“I’ve got an emergency”*
- *“I have a meeting”*
- *“I want to relax for a while without restrictions”*
- *“Super gentle quit”*

These reasons indicate users often **exit during a focus session due to interruptions**, not because they no longer want to use the app.

**Supporting evidence from MAU data:**
- Monthly active users completing **morning routines** is significantly higher than users completing **focus sessions**.
- This suggests that starting focus is a higher-friction step than completing routine activities.

**Screenshot referenced:**
- Quit Reasons dashboard showing app-quit event distribution

---

## Suggested Improvement to Reduce Drop-Off

### Introduce a “Pause & Resume Focus Session” flow

**Problem:**
Currently, when users are interrupted, quitting the session is the dominant path. This breaks momentum and reduces the likelihood of session completion.

**Proposed improvement:**
- Add a **Pause** option when a user attempts to quit a focus session
- Allow users to **resume** the session easily from the Home or Focus screen
- Treat interruptions as temporary, not failure states

**Why this should work:**
- Aligns directly with top quit reasons seen in PostHog
- Reduces all-or-nothing behaviour
- Increases chances of reaching the `completed-focus-session` event

**How to measure success in PostHog:**
- Reduction in `app-quit` during focus sessions
- Increase in `completed-focus-session`
- Increase in resume-related events
- Improved retention and stickiness for users who start focus sessions

---

## Reflection

### What user behaviour trend surprised me?
The gap between **routine completion** and **focus session completion** was larger than expected.  
Users are engaging with routines consistently but are more likely to drop off during focus, suggesting focus flows need stronger interruption support.

---

### How does PostHog data compare to customer feedback from Zoho Desk & Discord?
Customer feedback highlights:
- UI friction
- Timer interaction issues
- Permission and interruption frustration

PostHog confirms this at scale:
- Quit reasons cluster around interruption and restriction fatigue
- Focus completion is lower than expected relative to overall activity

Together, they point to focus sessions as the highest-impact area to improve.

---

### One improvement I’d suggest to Focus Bear based on analytics
Design focus sessions to be **interruption-tolerant**, not interruption-punitive.  
Supporting pause and recovery aligns the product with real user behaviour shown in PostHog and should improve completion, retention, and user trust.

---

## Summary
PostHog reveals that Focus Bear users are active and engaged, but interruptions during focus sessions are a key drop-off point. By addressing this with better pause and resume flows, Focus Bear can reduce abandonment, increase completed focus sessions, and improve long-term retention.
