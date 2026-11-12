# Work Distribution Document
## Axlero UI/UX Design (Figma) Internship — Group 1

**Document Version:** 1.0  
**Effective Date:** 8 November 2026  
**Submission Milestone:** Month 1 Mid Review Deliverable (Mandatory)  
**Lead Contact:** Arnav Arya (Team Lead) — `arnavarya2004@gmail.com`  
**GitHub Repository:** https://github.com/arnavarya001/Axlero.git  
**Figma Workspace (ShopVerse):** https://www.figma.com/design/pWC4bNgy8WBkMwjUTNR44P/ShopVerse-E-commerce?node-id=0-1&t=tJUJbAB72x5w3Vlf-1  

---

## 1. Executive Summary & Team Roster

This Work Distribution Document defines the architectural breakdown, task ownership, review schedules, and operational protocols for **Group 1** across both mandatory projects under the Axlero UI/UX Design Internship.

### Team Members & Assigned Branches

| No. | Member Name | Role in Team | GitHub Branch | Domain Focus |
|:---:|:---|:---|:---|:---|
| 1 | **Arnav Arya** | **Team Lead** | `arnav-lead` | Checkout flow, Vendor Dashboard, Git & Handoff |
| 2 | **Sudheer** | Team Member | `sudheer-research` | Personas, Customer Journey, Color Tokens, Product Cards |
| 3 | **Shashank Rao** | Team Member | `shashank-ia` | Information Architecture, User Flows, Typography, Icon Set |
| 4 | **Sajjad** | Team Member | `sajjad-wireframes` | Competitor Research, Home Wireframe, Button Systems |
| 5 | **Mukuture Kandji** | Team Member | `mukuture-wireframes` | PDP Wireframe, Input Components, Micro-interactions |

---

## 2. Review Dates & GitHub Compliance Milestones

| Milestone | Project Focus | Target Review Dates | Mandatory GitHub Rule | Status |
|:---|:---|:---|:---|:---:|
| **Month 1 Mid Review** | Project 1 (Weeks 1 & 2) | 23 Nov – 30 Nov 2026 | Commits on **at least 10 different days** in the 14 days prior | Scheduled |
| **Month 1 Final Review** | Project 1 (Weeks 3 & 4) | 5 Dec – 10 Dec 2026 *(TBC)* | **Commit on every single day (20 days)**, zero gaps allowed | Scheduled |
| **Month 2 Mid Review** | Project 2 (Weeks 1 & 2) | 23 Dec – 30 Dec 2026 | Commits on **at least 10 different days** in the 14 days prior | Scheduled |
| **Month 2 Final Review** | Project 2 (Weeks 3 & 4) | 5 Jan – 10 Jan 2027 *(TBC)* | **Commit on every single day (20 days)**, zero gaps allowed | Scheduled |

> **⚠️ Axlero Compliance Note:** Missing 2 commit days in the Final Review period leads to project invalidation. All members commit to their individual branches daily before 9:00 PM IST.

---

## 3. Month 1: Project 1 — Multi-Vendor Marketplace App (Mobile)
*Cycle: 8 Nov 2026 – 7 Dec 2026*  
*Target Platforms: iOS / Android Mobile-first Guidelines*

### Week 1: UX Research, Architecture & Grayscale Wireframes (8 – 15 Nov)
**Milestone Named Version:** `[Week 1] UX & Wireframes`

| Member | Specific Deliverables | Output Location |
|:---|:---|:---|
| **Arnav Arya (Lead)** | Repo scaffold, GitHub tracking, Vendor Dashboard wireframe, Checkout wireframes | `Axlero/`, `figma-versions/`, Figma `03_Wireframes` |
| **Sudheer** | Persona 1 "The Shopper", Shopper Journey Map (discovery to purchase) | `research/persona-shopper.md`, Figma `02_Research & Flows` |
| **Shashank Rao** | Information Architecture tree (Consumer & Vendor), Core Flow (Home ➔ Search ➔ PDP ➔ Cart) | `research/ia-and-flow.md`, Figma `02_Research & Flows` |
| **Sajjad** | Marketplace competitor analysis (Amazon, Meesho), Grayscale Home Page wireframe | `research/competitor-notes.md`, Figma `03_Wireframes` |
| **Mukuture Kandji** | Competitor bench-marking (Etsy, Flipkart), Product Detail Page (PDP) wireframe, Cart wireframe | `research/competitor-notes-2.md`, Figma `03_Wireframes` |

### Week 2: Design System & Scalable Component Library (16 – 22 Nov)
**Milestone Named Version:** `[Week 2] Design System`

| Member | Specific Deliverables | Output Location |
|:---|:---|:---|
| **Arnav Arya (Lead)** | 8pt Spacing tokens, layout grid setup, Top/Bottom Navigation Bar components, JSON token export | `design-tokens/tokens.json`, Figma `04_Design System` |
| **Sudheer** | Color variables (Primary, Secondary, Semantic alerts), WCAG AA contrast audit, Product Card component | `design-tokens/colors.json`, Figma `04_Design System` |
| **Shashank Rao** | Typography system (H1–H3, Body, Caption), SVG Icon library export (Home, Search, Cart, Heart, Profile) | `icons/*.svg`, Figma `04_Design System` |
| **Sajjad** | Interactive Button components with variants (Default, Hover, Active, Disabled, Sizes), Status Badges | `design-tokens/`, Figma `04_Design System` |
| **Mukuture Kandji** | Form Input components (Default, Focus, Active, Error states), Cart item card with quantity stepper | `design-tokens/`, Figma `04_Design System` |

### Week 3: High-Fidelity UI Screens & WCAG AA Verification (23 – 29 Nov)
**Milestone Named Version:** `[Week 3] Hi-Fi Screens`

| Member | Specific Deliverables | Output Location |
|:---|:---|:---|
| **Arnav Arya (Lead)** | Checkout 3-screen flow (Address ➔ Payment ➔ Confirmation), Stark contrast plugin audit, branch merges | Figma `05_High-Fidelity UI`, `accessibility-report.md` |
| **Sudheer** | Home screen Hi-Fi (Banner carousel, Flash deals, Vendor badges), Vendor Analytics screen | Figma `05_High-Fidelity UI` |
| **Shashank Rao** | Category Search & Filter screen Hi-Fi, Vendor "Add Product" form screen | Figma `05_High-Fidelity UI` |
| **Sajjad** | Product Detail Page (PDP) Hi-Fi with image slider, variant pills, and reviews section | Figma `05_High-Fidelity UI` |
| **Mukuture Kandji** | Cart screen Hi-Fi with coupon tray, Order Summary card, Empty state illustrations | Figma `05_High-Fidelity UI` |

### Week 4: Interactive Prototyping & Developer Handoff (30 Nov – 6 Dec)
**Milestone Named Version:** `[Week 4] Final Handoff`

| Member | Specific Deliverables | Output Location |
|:---|:---|:---|
| **Arnav Arya (Lead)** | Developer Handoff specifications, 8pt spacing redlines, final prototype audit, HM presentation prep | Figma `07_Developer Handoff`, `README.md` |
| **Sudheer** | End-to-end screen transitions (Home ➔ Search ➔ PDP), asset exports (SVG/PNG 1x, 2x, 3x) | Figma `06_Prototype`, `icons/` |
| **Shashank Rao** | Checkout flow interactive prototype, component design documentation | Figma `06_Prototype`, `07_Developer Handoff` |
| **Sajjad** | Micro-interactions: Heart favorite animation with Smart Animate, bottom tab animations | Figma `06_Prototype` |
| **Mukuture Kandji** | Button press micro-interactions, add-to-cart feedback drawer, Figma Mirror usability testing | `bug-list.md`, Figma `06_Prototype` |

---

## 4. Month 2: Project 2 — Telemedicine Patient Portal (Web)
*Cycle: 8 Dec 2026 – 7 Jan 2027*  
*Target Platform: Accessible Web Dashboard (WCAG 2.1 AA)*

### Week 1: Empathy Mapping, A11y Research & Booking Flows (8 – 15 Dec)
**Milestone Named Version:** `[Week 1] A11y Wireframes`
- **Sudheer:** Persona "Elderly Patient with Chronic Care Needs", Symptom input wireframes.
- **Shashank Rao:** Patient Empathy Map, Step-by-step progressive disclosure booking flow (Doctor ➔ Date ➔ Symptoms ➔ Confirm).
- **Sajjad:** Telehealth competitor research (Practo, Teladoc), Patient Dashboard wireframe.
- **Mukuture Kandji:** Accessibility guidelines (contrast 4.5:1, min 48px touch targets, 16px+ base font), Doctor Search wireframe.
- **Arnav Arya (Lead):** Project 2 setup, Calendar date-picker wireframe, consultation room layout wireframe.

### Week 2: Medical UI Kit & Scalable Iconography (16 – 22 Dec)
**Milestone Named Version:** `[Week 2] Medical UI Kit`
- **Sudheer:** Calming healthcare palette (therapeutic blues & sage greens), contrast test matrix.
- **Shashank Rao:** High-legibility web typography scale, Step progress bar component.
- **Sajjad:** Large-target form inputs, appointment cards, doctor profile cards with nested Auto-Layout.
- **Mukuture Kandji:** Medical SVG icon library (Stethoscope, Prescription, Video Call, Heartbeat, Calendar).
- **Arnav Arya (Lead):** Video call controls component (Mute, Camera, Screen Share, Chat tray), Alert banners.

### Week 3: High-Fidelity Web Dashboard (23 – 29 Dec)
**Milestone Named Version:** `[Week 3] Hi-Fi Dashboard`
- **Sudheer:** Patient Dashboard screen (Upcoming visits, Medication reminders, Recent test summaries).
- **Shashank Rao:** 4-step Appointment Booking flow screens (High-Fidelity).
- **Sajjad:** Prescription history & downloadable PDF summary screen.
- **Mukuture Kandji:** Active Video Consultation screen with doctor video feed and real-time chat side-panel.
- **Arnav Arya (Lead):** Lab test results screen, accessibility verification using axe / Stark plugin.

### Week 4: Edge Cases, Usability Testing & Developer Handoff (30 Dec – 6 Jan)
**Milestone Named Version:** `[Week 4] Final Handoff`
- **Sudheer & Shashank Rao:** Edge cases design (Doctor is running late, Video connection dropped modal, session reconnect).
- **Sajjad & Mukuture Kandji:** Usability testing session with real elderly participants, usability feedback documentation.
- **Arnav Arya (Lead):** Developer handoff specifications, final clickable prototype, 20-day commit audit.

---

## 5. Daily Commit Rota Schedule

To prevent any single point of failure in daily GitHub activity, each day has a designated **Owner** and **Backup**:

| Day of Week | Primary Owner | Backup Owner | Daily Cutoff | Fallback Action |
|:---|:---|:---|:---:|:---|
| **Monday** | Sudheer | Arnav Arya | 9:00 PM IST | If Owner misses by 9 PM, Backup commits by 10 PM |
| **Tuesday** | Shashank Rao | Sudheer | 9:00 PM IST | If Owner misses by 9 PM, Backup commits by 10 PM |
| **Wednesday** | Sajjad | Shashank Rao | 9:00 PM IST | If Owner misses by 9 PM, Backup commits by 10 PM |
| **Thursday** | Mukuture Kandji | Sajjad | 9:00 PM IST | If Owner misses by 9 PM, Backup commits by 10 PM |
| **Friday** | Arnav Arya | Mukuture Kandji | 9:00 PM IST | If Owner misses by 9 PM, Backup commits by 10 PM |
| **Saturday** | Sudheer | Shashank Rao | 9:00 PM IST | If Owner misses by 9 PM, Backup commits by 10 PM |
| **Sunday** | Shashank Rao | Arnav Arya | 9:00 PM IST | If Owner misses by 9 PM, Backup commits by 10 PM |

---

## 6. Unresponsive Member & Escalation Protocol

In strict accordance with Section 6 of the Axlero Project Execution Handbook:

```
[Member Unresponsive]
       │
       ▼
Step 1: Contact via all channels (WhatsApp call/message, Email, Discord).
       │
       ▼
Step 2: Allow strict 48-Hour Grace Window.
       │
       ├──► If member responds: Realign task deadlines immediately.
       │
       └──► If NO response after 48 hours:
             │
             ▼
Step 3: Lead informs Axlero Mentors with screenshot evidence.
       │
       ▼
Step 4: Active members redistribute tasks; unresponsive member marked inactive
        and evaluated separately by Axlero management.
```

---

## 7. Team Sign-Off & Confirmation

By confirming below, each team member acknowledges their assigned deliverables, the mandatory daily commit schedule, and the review milestones:

| Team Member | Role | Branch | Confirmation Status | Date |
|:---|:---|:---|:---:|:---:|
| **Arnav Arya** | Team Lead | `arnav-lead` | **Confirmed (Lead)** | 11 Nov 2026 |
| **Sudheer** | Team Member | `sudheer-research` | *Pending WhatsApp Reply* | — |
| **Shashank Rao** | Team Member | `shashank-ia` | *Pending WhatsApp Reply* | — |
| **Sajjad** | Team Member | `sajjad-wireframes` | *Pending WhatsApp Reply* | — |
| **Mukuture Kandji** | Team Member | `mukuture-wireframes` | *Pending WhatsApp Reply* | — |

---
*Submitted on behalf of Axlero UI/UX Group 1 by Arnav Arya (Team Lead).*

