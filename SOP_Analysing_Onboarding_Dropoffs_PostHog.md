# SOP: Analysing Onboarding & Drop-Offs Using PostHog

## Document Purpose

This Standard Operating Procedure (SOP) explains how to use PostHog at Focus Bear to analyse user behaviour during sign-up and onboarding, identify drop-off points, and translate analytics into actionable product insights.

This SOP is intended for Product Managers, interns, and team members who need a repeatable and reliable way to use analytics to inform product decisions.

---

## When to Use PostHog (and When Not To)

### Use PostHog when:
- You want to understand what users are actually doing, not just what they say
- You need to identify drop-off points in onboarding or key flows
- You want to validate whether a UX change improved behaviour
- You are analysing trends across many users (quantitative insights)

### Do NOT rely only on PostHog when:
- You need context, emotions, or motivations → use Zoho Desk or Discord
- The issue affects a very small number of users → support tickets are better

**Best practice:**  
Use PostHog for behaviour patterns, then validate findings with support feedback.

---

## Tools & Access Required

- Access to Focus Bear’s PostHog workspace  
- Read access is sufficient  
- Browser with ability to take screenshots  

---

## Key Metrics PMs Should Track in PostHog

When analysing onboarding or early usage, focus on:

- Sign-up funnel completion
- Onboarding step completion rates
- Time taken between steps
- Drop-off percentages per step
- Event frequency (e.g. focus session started)
- Platform segmentation (Android, iOS, Web if applicable)

Avoid vanity metrics. Focus on behaviour that maps directly to user value.

---

## Step-by-Step: How to Analyse Onboarding Using PostHog

### Step 1: Open Relevant Dashboards
- Log in to PostHog
- Navigate to **Dashboards**
- Open onboarding or funnel-related dashboards (e.g. sign-up → first action)
- If no dashboard exists, use **Funnels** to create one

---

### Step 2: Review the Onboarding Funnel

Identify key steps, such as:
- Account created
- Onboarding completed
- First focus session started

Observe:
- Percentage drop-off at each step
- Largest single drop-off point
- Sudden behaviour changes between steps

---

### Step 3: Identify One Clear Drop-Off Point

Choose **one meaningful drop-off**, not multiple.

Examples:
- Large drop between “App opened” → “Focus session started”
- High abandonment during permissions or setup steps

This keeps analysis focused and actionable.

---

### Step 4: Segment the Data (Optional but Recommended)

Where possible, segment by:
- Platform (Android / iOS)
- New vs returning users
- Time period (before / after a change)

This helps determine whether the issue is systemic or platform-specific.

---

### Step 5: Take Evidence Screenshots

For each insight:
- Take a screenshot showing:
  - Funnel steps
  - Drop-off percentages
  - Date range
- Ensure numbers are clearly visible

Screenshots act as proof and help others validate findings.

---

## Turning Data Into Product Insights

Analytics alone are not enough. Always connect data to user experience.

Ask these questions:
- Why might users be dropping off here?
- Is this step cognitively heavy or unclear?
- Does this align with recent user feedback?
- Is this expected or surprising behaviour?

---

## Suggesting a Product Improvement

Each PostHog analysis should end with **one clear suggestion**.

**Structure:**
- **Observed behaviour:** What the data shows  
- **Likely cause:** UX, clarity, friction, permissions, etc.  
- **Suggested improvement:** Small, testable change  

**Example:**

Users drop off heavily before starting their first focus session. This aligns with support feedback indicating uncertainty around distraction blocking. A short preview explaining what will be blocked before starting focus could reduce hesitation.

---

## Documenting Findings

Save insights in Markdown using this structure:
- Goal of analysis
- Funnel reviewed
- Drop-off identified (with screenshot)
- Insight summary
- Suggested improvement

This ensures findings are reusable and easy to review.

---

## Common Mistakes to Avoid

- Analysing too many funnels at once
- Reporting numbers without interpretation
- Making assumptions without user context
- Ignoring screenshots or evidence
- Suggesting large solutions without validating root cause

---

## Expected Outcome

Following this SOP should result in:
- Clear identification of onboarding friction
- Evidence-backed product recommendations
- Alignment between analytics and support feedback
- Faster decision-making with less guesswork

---

## Final Note

PostHog is most powerful when used consistently and thoughtfully. This SOP ensures that anyone analysing user behaviour at Focus Bear follows the same structured approach, reducing confusion and increasing the quality of insights.
