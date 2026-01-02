## Wireframe / Annotated User Journey (Annotated Visual Flow)

Below is a step-by-step annotated representation of the user journey, referencing specific screen elements and layout zones to act as a visual guide for developers and designers.

### Screen 1: Welcome / Greeting Screen
- **Top area (Header):**
  - Current issue: Greeting text (“Hi [email]”) is partially hidden by the system status bar.
  - Proposed change: Add safe-area padding and replace email greeting with nickname input during onboarding.
- **Visual reference:** Header container + greeting text area.

---

### Screen 2: Home → Overview
- **Top navigation bar:**
  - Issue: App title and health status icons appear truncated or visually crowded on smaller screens.
  - Proposed change: Increase top padding and enforce consistent spacing rules across screens.
- **Visual reference:** App title, status icons, and top container alignment.

---

### Screen 3: Focus Tab (Timer Selection)
- **Timer selector (scroll wheel):**
  - Issue:
    - Scroll wheel stops abruptly instead of looping naturally.
    - Timer formatting shows unclear values (e.g. “55..”).
  - Proposed change:
    - Infinite looping scroll (native picker behaviour).
    - Clean numeric formatting (e.g. “55 min”).
- **Visual reference:** Timer picker component and numeric labels.

---

### Screen 4: Focus Session (Super Strict Mode Enabled)
- **Session start state:**
  - Issue: UI issues persist regardless of mode, indicating shared layout components.
  - Proposed change: Apply layout fixes globally across all modes.
- **Visual reference:** Focus session screen with strict mode indicator.

---

### Screen 5: Stats Tab
- **Header & spacing:**
  - Issue: Header text competes visually with system UI.
  - Proposed change: Consistent spacing and typography hierarchy across all tabs.
- **Visual reference:** Stats screen header and content container.

---

### Summary Visual Flow
Login → Welcome Screen → Home Overview → Focus Timer Selection → Active Focus Session → Stats Review

Each step highlights where visual clarity, spacing, and predictability can be improved to reduce cognitive load and improve onboarding confidence.
