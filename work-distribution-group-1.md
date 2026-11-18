# Work Distribution Document
## Axlero UI/UX Design (Figma) Internship — Group 1

**Document Version:** 1.2  
**Effective Date:** 8 November 2026  
**Last Updated:** 18 November 2026 (Week 2 Design System Phase)  
**Submission Milestone:** Month 1 Mid Review Deliverable (Mandatory)  
**Lead Contact:** Arnav Arya (Team Lead) — `arnavarya2004@gmail.com`  
**GitHub Repository:** https://github.com/arnavarya001/Axlero.git  

---

## 🔗 Official Figma Workspaces

In accordance with Axlero PRD Section 8, all evaluations are conducted from a single consolidated master Figma project:

| Workspace Role | Project Title | Direct Figma Link | Status |
|:---|:---|:---|:---:|
| **⭐ Master Team File** | **ShopVerse - E-commerce** | [Open ShopVerse Master](https://www.figma.com/design/pWC4bNgy8WBkMwjUTNR44P/ShopVerse-E-commerce?node-id=71-74&t=0plpW883l0ZShwDn-1) | **Primary Evaluation File** |
| **Lead Scaffold File** | **Axlero - P1 Marketplace** | [Open Axlero P1 Scaffold](https://www.figma.com/design/heSsWnpBLEQYwlNRyqAW5t/Axlero---P1-Marketplace?node-id=1-3&t=DzAsycyWk2ZoRiJE-1) | Lead Reference |
| **Lead Scratch File** | **ShopVerse Explorations** | [Open Explorations](https://www.figma.com/design/mzxRxVZF9eTfuu8vupSgu7/Untitled?node-id=2-7&t=Lylrka5IOSHXPiPW-1) | Flow Wireframes |

> **Consolidation Directive:** By the end of Week 2 (22 Nov), all frames from the Lead scaffold files are being merged into **ShopVerse - E-commerce** so that evaluators see all 7 pages and member contribution history in one place.

---

## 1. Executive Summary & Team Roster

This Work Distribution Document defines the architectural breakdown, task ownership, review schedules, and operational protocols for **Group 1** across both mandatory projects under the Axlero UI/UX Design Internship.

### Team Members & Assigned Branches

| No. | Member Name | Role in Team | GitHub Branch | Domain Focus |
|:---:|:---|:---|:---|:---|
| 1 | **Arnav Arya** | **Team Lead** | `arnav-lead` | Checkout flow (3-screen rule), Vendor Dashboard, Tokens & Merges |
| 2 | **Sudheer** | Team Member | `sudheer-research` | Personas, Customer Journey, Color Tokens, Product Cards |
| 3 | **Shashank Rao** | Team Member | `shashank-ia` | Information Architecture, User Flows, Typography, Icon Set |
| 4 | **Sajjad Dhuka** | Team Member | `sajjad-wireframes` | Competitor Research, Home Wireframe, Button System, PDP states |
| 5 | **Mukuture Kandji** | Team Member | `mukuture-wireframes` | PDP Wireframe, Input Components, Prototype Micro-interactions |

---

## 2. Review Dates & GitHub Compliance Milestones

| Milestone | Project Focus | Target Review Dates | Mandatory GitHub Rule | Current Status |
|:---|:---|:---|:---|:---:|
| **Month 1 Mid Review** | Project 1 (Weeks 1 & 2) | 24 Nov – 30 Nov 2026 | Commits on **at least 10 different days** in the 14 days prior | **On Track (5 / 10 days met as of 18 Nov)** |
| **Month 1 Final Review** | Project 1 (Weeks 3 & 4) | 5 Dec – 10 Dec 2026 *(TBC)* | **Commit on every single day (20 days)**, zero gaps allowed | Scheduled |
| **Month 2 Mid Review** | Project 2 (Weeks 1 & 2) | 23 Dec – 30 Dec 2026 | Commits on **at least 10 different days** in the 14 days prior | Scheduled |
| **Month 2 Final Review** | Project 2 (Weeks 3 & 4) | 5 Jan – 10 Jan 2027 *(TBC)* | **Commit on every single day (20 days)**, zero gaps allowed | Scheduled |

### ⚠️ Commit Audit & Mid Review Strategy (As of 18 Nov 2026)
- **Commits Logged So Far:** 11 Nov (Lead), 12 Nov (Lead), 14 Nov (Sajjad), 16 Nov (Mukuture), 17 Nov (Sajjad), 18 Nov (Lead). Total: **5 distinct commit days**.
- **Action Plan:** To clear the 10-day requirement, the team must commit consecutively on 19, 20, 21, 22, 23, and 24 Nov. Arnav has targeted the Mid Review slot between **24 Nov and 28 Nov** to guarantee full compliance before the mentor evaluation.

---

## 3. Month 1: Project 1 — Multi-Vendor Marketplace App (Mobile)
*Cycle: 8 Nov 2026 – 7 Dec 2026*  
*Target Platforms: iOS / Android Mobile-first Guidelines (390 × 844 viewport)*

### Week 1: UX Research, Architecture & Grayscale Wireframes (8 – 15 Nov)
**Milestone Named Version:** `[Week 1] UX & Wireframes`

| Member | Specific Deliverables | Output Location | Status |
|:---|:---|:---|:---:|
| **Arnav Arya (Lead)** | Repo scaffold, GitHub tracking, Vendor Dashboard wireframe, Checkout wireframes | `Axlero/`, `figma-versions/`, Figma `03_Wireframes` | Completed |
| **Sudheer** | Persona 1 "The Shopper", Shopper Journey Map (discovery to purchase) | `research/persona-shopper.md`, Figma `02_Research & Flows` | In Progress |
| **Shashank Rao** | Information Architecture tree (Consumer & Vendor), Core Flow (Home ➔ Search ➔ PDP ➔ Cart) | `research/ia-and-flow.md`, Figma `02_Research & Flows` | In Progress |
| **Sajjad Dhuka** | Marketplace competitor analysis (Amazon, Meesho), Grayscale Home Page wireframe, Category Search | `research/competitor-notes.md`, Figma `03_Wireframes` | Completed |
| **Mukuture Kandji** | Competitor bench-marking (Etsy, Flipkart), Product Detail Page (PDP) wireframe, Cart wireframe | `research/competitor-notes-2.md`, Figma `03_Wireframes` | Completed |

### Week 2: Design System & Scalable Component Library (16 – 22 Nov) — ACTIVE
**Milestone Named Version:** `[Week 2] Design System`

| Member | Specific Deliverables | Output Location | Status |
|:---|:---|:---|:---:|
| **Arnav Arya (Lead)** | Exported Design Tokens (`tokens.json`, `tokens.css`), 8pt Spacing tokens, layout grid setup | `design-tokens/`, Figma `04_Design System` | Completed |
| **Sudheer** | Color variables (Primary, Secondary, Semantic alerts), WCAG AA contrast audit, Product Card component | `design-tokens/`, Figma `04_Design System` | In Progress |
| **Shashank Rao** | Typography system (H1–H3, Body, Caption), SVG Icon library export (Home, Search, Cart, Heart, Profile) | `icons/*.svg`, Figma `04_Design System` | In Progress |
| **Sajjad Dhuka** | Button components with variants (Default, Hover, Active, Disabled, Sizes), Status Badges, PDP States | `screenshots/`, Figma `04_Design System` | Completed |
| **Mukuture Kandji** | Form Input components (Default, Focus, Active, Error states), Cart item card with quantity stepper | `design-tokens/`, Figma `04_Design System` | In Progress |

### Week 3: High-Fidelity UI Screens & WCAG AA Verification (23 – 29 Nov)
**Milestone Named Version:** `[Week 3] Hi-Fi Screens`
- **Arnav Arya (Lead):** Checkout 3-screen flow (Address ➔ Payment ➔ Confirmation), Stark contrast audit, branch PR merges.
- **Sudheer:** Home screen Hi-Fi (Banner carousel, Flash deals, Vendor badges), Vendor Analytics screen.
- **Shashank Rao:** Category Search & Filter screen Hi-Fi, Vendor "Add Product" form screen.
- **Sajjad Dhuka:** Product Detail Page (PDP) Hi-Fi with image slider, variant pills, and reviews section.
- **Mukuture Kandji:** Cart screen Hi-Fi with coupon tray, Order Summary card, Empty state illustrations.

### Week 4: Interactive Prototyping & Developer Handoff (30 Nov – 6 Dec)
**Milestone Named Version:** `[Week 4] Final Handoff`
- **Arnav Arya (Lead):** Developer Handoff specifications, 8pt spacing redlines, final prototype audit, HM defense prep.
- **Sudheer:** End-to-end screen transitions (Home ➔ Search ➔ PDP), asset exports (SVG/PNG 1x, 2x, 3x).
- **Shashank Rao:** Checkout flow interactive prototype, component design documentation.
- **Sajjad Dhuka:** Micro-interactions: Heart favorite animation with Smart Animate, bottom tab animations.
- **Mukuture Kandji:** Button press micro-interactions, add-to-cart feedback drawer, Figma Mirror usability testing.

---

## 4. Month 2: Project 2 — Telemedicine Patient Portal (Web)
*Cycle: 8 Dec 2026 – 7 Jan 2027*  
*Target Platform: Accessible Web Dashboard (WCAG 2.1 AA)*

- **Week 1 (8 – 15 Dec):** Empathy Mapping, A11y Research & Booking Flows. Named Version: `[Week 1] A11y Wireframes`.
- **Week 2 (16 – 22 Dec):** Medical UI Kit & Scalable Iconography. Named Version: `[Week 2] Medical UI Kit`.
- **Week 3 (23 – 29 Dec):** High-Fidelity Web Dashboard (Upcoming visits, Prescriptions, Video consultation). Named Version: `[Week 3] Hi-Fi Dashboard`.
- **Week 4 (30 Dec – 6 Jan):** Edge Cases, Error States & Usability Testing. Named Version: `[Week 4] Final Handoff`.

---

## 5. Daily Commit Rota Schedule

To prevent any single point of failure in daily GitHub activity, each day has a designated **Owner** and **Backup**:

| Day of Week | Primary Owner | Backup Owner | Daily Cutoff | Fallback Action |
|:---|:---|:---|:---:|:---|
| **Monday** | Sudheer | Arnav Arya | 9:00 PM IST | If Owner misses by 9 PM, Backup commits by 10 PM |
| **Tuesday** | Shashank Rao | Sudheer | 9:00 PM IST | If Owner misses by 9 PM, Backup commits by 10 PM |
| **Wednesday** | Sajjad Dhuka | Shashank Rao | 9:00 PM IST | If Owner misses by 9 PM, Backup commits by 10 PM |
| **Thursday** | Mukuture Kandji | Sajjad Dhuka | 9:00 PM IST | If Owner misses by 9 PM, Backup commits by 10 PM |
| **Friday** | Arnav Arya | Mukuture Kandji | 9:00 PM IST | If Owner misses by 9 PM, Backup commits by 10 PM |
| **Saturday** | Sudheer | Shashank Rao | 9:00 PM IST | If Owner misses by 9 PM, Backup commits by 10 PM |
| **Sunday** | Shashank Rao | Arnav Arya | 9:00 PM IST | If Owner misses by 9 PM, Backup commits by 10 PM |

---

## 6. Unresponsive Member & Escalation Protocol

In strict accordance with Section 6 of the Axlero Project Execution Handbook:
1. **Step 1:** Contact member via all channels (WhatsApp call/message, Email).
2. **Step 2:** Allow strict 48-Hour Grace Window.
3. **Step 3:** If no response, inform Axlero Mentors with screenshot evidence.
4. **Step 4:** Active members redistribute remaining tasks; unresponsive member marked inactive and evaluated separately.

---

## 7. Team Sign-Off & Confirmation

| Team Member | Role | Branch | Confirmation Status | Date |
|:---|:---|:---|:---:|:---:|
| **Arnav Arya** | Team Lead | `arnav-lead` | **Confirmed (Lead)** | 18 Nov 2026 |
| **Sudheer** | Team Member | `sudheer-research` | Confirmed | 14 Nov 2026 |
| **Shashank Rao** | Team Member | `shashank-ia` | Confirmed | 14 Nov 2026 |
| **Sajjad Dhuka** | Team Member | `sajjad-wireframes` | **Active Contributor** | 17 Nov 2026 |
| **Mukuture Kandji** | Team Member | `mukuture-wireframes` | **Active Contributor** | 16 Nov 2026 |

---
*Submitted on behalf of Axlero UI/UX Group 1 by Arnav Arya (Team Lead).*
