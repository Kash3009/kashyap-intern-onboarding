## Understanding How the Backlog Works at Focus Bear (Based on Direct GitHub Access)

### When & How I Reviewed the Backlog

on 8th Jan 2026 I reviewed the **Focus Bear GitHub Projects → Mobile App Tasks** board after receiving full access to the repository.

I explored the board in **Board view**, scrolling through multiple columns to understand:
- How work is categorised
- How priority is communicated
- How blocked, future, and urgent items are handled

I specifically reviewed the following columns:
- Development paused – waiting for upstream dependencies  
- Unprioritised – don’t touch for now  
- Jan 2026  
- Q1 2026  
- 2026  
- 2027  
- Emergency fix needed  

Screenshots of each column reviewed are attached below and referenced in this document.

---

## Backlog Tool Used

Focus Bear manages its backlog using **GitHub Projects**, with:
- Individual **GitHub Issues** as backlog items
- A **shared Project board** for prioritisation and visibility
- Labels to indicate platform (mobile-app, backend, web-dashboard) and type (bug, UI, idea, project)

---

## Types of Backlog Items (Observed in Focus Bear’s Backlog)

Based on direct observation of the **Mobile App Tasks** board, three clear backlog item types are used.

### 1. Bug Fixes

These represent issues where existing functionality is broken or unreliable and often appear in **Emergency fix needed** or near-term columns.

**Examples observed:**
- **mobile-app #1399** – *Error: Foreground service fails to stop*  
  - Status: Development paused – waiting for upstream dependencies  
- **mobile-app #3729** – *Sentry errors*  
  - Status: Emergency fix needed  

These items directly impact reliability and user trust and are clearly treated as high priority.

Screenshot reference:  <img width="788" height="558" alt="image" src="https://github.com/user-attachments/assets/293dcc0c-7fd6-46e6-9dd4-e4347fb57832" />
<img width="390" height="508" alt="image" src="https://github.com/user-attachments/assets/29fe9c46-5723-444a-8a7e-eca5f465e6d7" />

---

### 2. Feature Requests / Ideas

These represent new capabilities or behavioural changes and are typically scheduled into future time buckets.

**Examples observed:**
- **mobile-app #2734** – *[IDEA] Geofencing – trigger custom routines*  
  - Status: 2027  
  - Label: needs-refinement  
- **mobile-app #1953** – *Support pomodoro mode on mobile*  
  - Status: Q1 2026  

These items are acknowledged but intentionally deferred until scope, feasibility, or priority becomes clearer.

Screenshot reference: <img width="377" height="534" alt="image" src="https://github.com/user-attachments/assets/bd9fd89c-fc8f-4c30-ab22-27b6fac09d03" />
<img width="398" height="550" alt="image" src="https://github.com/user-attachments/assets/6b1ce8b1-ed53-4eca-925b-cbfa906e49b1" />


---

### 3. UX / UI Improvements

These focus on usability, clarity, and accessibility rather than core logic.

**Examples observed:**
- **mobile-app #710** – *[UI] Changes to manage apps UI design*  
  - Status: Development paused – waiting for upstream dependencies  
- **mobile-app #883** – *Selected time from Set Startup Time window will be reflected on the succeeding windows*  
  - Status: Unprioritised – don’t touch for now  

These improvements reduce friction, especially for Focus Bear’s neurodivergent users.

Screenshot reference: <img width="385" height="519" alt="image" src="https://github.com/user-attachments/assets/586ec0fd-91cc-4c08-92f4-c0a462fda365" />
<img width="388" height="520" alt="image" src="https://github.com/user-attachments/assets/57ab54a8-ce52-42c1-8145-b0090b7d8036" />


---

## How Backlog Items Move Through the Workflow

Based on direct observation of issue movement and column usage, backlog items typically follow this flow:

### 1. Issue Logged
An issue is created in GitHub by a developer, PM, QA, or via surfaced user feedback.

**Example:**  
- mobile-app #2734 – *[IDEA] Geofencing – trigger custom routines*

---

### 2. Categorisation
The issue is:
- Tagged by platform (mobile-app, backend, web-dashboard)
- Labelled by type (bug, UI, idea, project)
- Added to the Mobile App Tasks board

---

### 3. Refinement
Some issues receive labels such as **needs-refinement**, indicating:
- Scope is unclear
- Acceptance criteria are missing
- Technical approach needs discussion

---

### 4. Prioritisation & Scheduling
Instead of fixed sprints, Focus Bear uses **time-based prioritisation columns**, including:
- Unprioritised – don’t touch for now
- Jan 2026
- Q1 2026
- 2026
- 2027

This keeps future work visible without forcing premature commitment.

Screenshot reference: <img width="398" height="554" alt="image" src="https://github.com/user-attachments/assets/12a2a167-87fe-4d92-aedb-b9a18ed382e7" />
<img width="365" height="527" alt="image" src="https://github.com/user-attachments/assets/747a91be-2813-4a7f-98ec-2490fae994a6" />
<img width="385" height="528" alt="image" src="https://github.com/user-attachments/assets/6540c169-7cc8-483d-a400-5d6ff03be34d" />



---

### 5. Blocked / Paused Work
Items blocked by dependencies are explicitly tracked.

**Example:**
- **mobile-app #3276** – *Replace pusher beams with firebase cloud messenger*  
  - Status: Development paused – waiting for upstream dependencies  

This prevents blocked work from being forgotten.

Screenshot reference: <img width="388" height="518" alt="image" src="https://github.com/user-attachments/assets/8f52cffc-e5e3-48ee-a5c6-f4cf46187ed6" />


---

### 6. Active Development → QA → Completion
Once prioritised and unblocked:
- Work moves into development
- Is tested and validated
- Then closed, with history preserved in GitHub Issues

---

## Reflection

### What I Noticed About the Backlog Structure

- Priority is **explicit and visible**
- Blocked work is clearly separated
- Future ideas are tracked without pressure to execute immediately
- Mobile, backend, and web work coexist without losing clarity

---

### Challenges Observed

- Balancing urgent bugs with long-term feature ideas
- Preventing items in *Unprioritised* or far-future columns from stagnating
- Ensuring sufficient refinement before work is pulled into development

---

### One Improvement I’d Suggest

Add a lightweight refinement checklist for items entering future-dated columns:
- Clear problem statement
- User impact
- Acceptance criteria
- Known dependencies

This would reduce clarification overhead when items are eventually picked up.

---

## Summary

By directly reviewing the **Mobile App Tasks GitHub Project**, it’s clear that Focus Bear manages its backlog through continuous prioritisation, explicit status signalling, and strong visibility across bugs, features, and UX improvements.

This structure supports fast iteration while keeping long-term work visible and controlled.
