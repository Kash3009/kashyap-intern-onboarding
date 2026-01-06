## Understanding How the Backlog Works (Based on Direct GitHub Access)

After receiving access to Focus Bear’s GitHub Projects, I reviewed the **Mobile App Tasks** board, which is the primary backlog used by the mobile team. This summary is based on direct observation of real backlog items, their labels, and how they are organised across workflow columns such as *Development paused*, *Unprioritised*, and future time buckets (e.g. 2026, Q1 2026, 2027).

This provides a concrete understanding of how the Focus Bear backlog actually functions in practice and how items move from idea to implementation.

---

## What Is a Product Backlog?

At Focus Bear, the product backlog lives in **GitHub Projects** and represents all work that may be built in the future. This includes bugs, feature ideas, UX improvements, and technical work across mobile, backend, and web.

Unlike a roadmap, which communicates long-term direction and timelines, the backlog is a **tactical, operational tool** that:
- Changes frequently
- Reflects real engineering constraints
- Supports continuous prioritisation rather than fixed sprint commitments

For a startup like Focus Bear, the backlog enables:
- Fast iteration  
- Clear visibility into work status  
- Prioritisation based on impact, urgency, and feasibility  

---

## Types of Backlog Items (Observed in Focus Bear’s Backlog)

Reviewing the **Mobile App Tasks** board shows three clear types of backlog items.

### 1. Bug Fixes

These are issues where existing functionality does not behave as expected.

**Examples:**
- `mobile-app #1399 – Error: Foreground service fails to stop`
- `mobile-app #3729 – Sentry errors`

These items directly impact reliability or user experience and are often prioritised higher, especially when they block users or cause crashes.

---

### 2. Feature Requests / Ideas

These are new capabilities or behavioural changes that extend the product.

**Examples:**
- `mobile-app #2734 – [IDEA] Geofencing – trigger custom routines`
- `mobile-app #1953 – Support pomodoro mode on mobile`

Feature ideas are often placed into future time buckets (e.g. 2027 or Q1 2026) and may be labelled `needs-refinement`, indicating they are acknowledged but not yet ready for development.

---

### 3. UX / UI Improvements

These focus on usability, accessibility, and clarity rather than core functionality.

**Examples:**
- `mobile-app #710 – [UI] Changes to manage apps UI design`
- `mobile-app #883 – Selected time from Set Startup Time window will be reflected on the succeeding windows`

These items improve consistency and reduce friction, which is especially important for Focus Bear’s neurodivergent user base.

---

## How Backlog Items Move Through Focus Bear’s Workflow

Based on direct observation of the Mobile App Tasks board, backlog items typically move through the following stages.

### 1. Idea or Issue Logged

An item is created as a GitHub Issue by a developer, PM, QA, or through surfaced user feedback.

**Example:**
- `mobile-app #2734 – [IDEA] Geofencing – trigger custom routines`

---

### 2. Initial Categorisation

The issue is:
- Tagged by platform (mobile-app, backend, web-dashboard)
- Labelled by type (bug, idea, UI, project)
- Added to the Mobile App Tasks board

---

### 3. Refinement

Some items receive additional context, comments, or labels such as `needs-refinement`.  
This indicates the scope, acceptance criteria, or technical approach still needs clarification before development can begin.

---

### 4. Prioritisation & Scheduling

Instead of fixed sprints, Focus Bear uses **time-based prioritisation columns**, such as:
- *Unprioritised – don’t touch for now*
- *2026*
- *Q1 2026*
- *2027*

This keeps future work visible while allowing flexibility.

---

### 5. Blocked or Paused Work

Items that cannot proceed due to external dependencies move into:

**Development paused – waiting for upstream dependencies**

**Example:**
- `mobile-app #3276 – Replace pusher beams with firebase cloud messenger`

This ensures blocked work is tracked rather than forgotten.

---

### 6. Active Development → QA → Completion

Once prioritised and unblocked, items move into development, are tested, and eventually closed. Completed work remains accessible through GitHub issue history.

---

## Reflection

### What I Noticed About the Backlog Structure

The backlog is:
- Transparent about priority and status
- Organised around continuous prioritisation
- Explicit about blocked work and future ideas
- Shared across platforms while allowing mobile-specific focus

This structure supports rapid iteration without losing visibility of long-term work.

---

### Challenges in Backlog Management

Some challenges that stand out include:
- Balancing urgent bugs with long-term feature ideas
- Preventing unprioritised items from stagnating
- Ensuring adequate refinement before development starts
- Coordinating work across multiple platforms

---

### One Improvement I Would Suggest

Introduce a lightweight refinement checklist for items entering future-dated columns, including:
- Clear problem statement
- User impact
- Acceptance criteria
- Known dependencies

This would reduce clarification overhead and speed up development when items are picked up.

---

## Summary

By reviewing the **Mobile App Tasks** GitHub Project, it’s clear that Focus Bear manages its backlog through continuous prioritisation, clear status signalling, and strong visibility across bugs, features, and UX improvements. Understanding how real backlog items move from idea → refinement → prioritisation → development provides a solid foundation for effective product management at Focus Bear.
