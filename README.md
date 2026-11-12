# Axlero UI/UX Design Internship - Group 1

Welcome to the official repository for **Axlero UI/UX Design Internship (Group 1)**. This repository hosts UX research documentation, exported design tokens, SVG icon assets, and tracked Figma Named Versions.

---

## 👥 Team Members & Roles

| Member | Role | GitHub Branch | Focus Area |
| :--- | :--- | :--- | :--- |
| **Arnav Arya** | Team Lead | `arnav-lead` | Checkout flow, Vendor Dashboard, Coordination & Merges |
| **Sudheer** | Team Member | `sudheer-research` | Personas, Shopper Journey, Product Card, Color Tokens |
| **Shashank Rao** | Team Member | `shashank-ia` | Information Architecture, User Flows, Typography, Iconography |
| **Sajjad** | Team Member | `sajjad-wireframes` | Home Page Wireframe, Competitor Analysis, Button System |
| **Mukuture Kandji** | Team Member | `mukuture-wireframes` | PDP Wireframe, Input Components, Prototype Micro-interactions |

---

## 📱 Projects Overview

### Project 1: Multi-Vendor Marketplace App (Mobile)
- **Duration:** 8 Nov 2026 – 7 Dec 2026
- **Focus:** Mobile-first consumer shopping application (Home, Search, PDP, Cart, Checkout) & Vendor Management Dashboard.
- **Key UX Requirements:**
  - Maximum 3 screens from "Add to Cart" to "Order Confirmed".
  - 100% Auto-Layout across all frames and components.
  - WCAG AA color contrast compliance.
  - No detached components or raw hex codes.

### Project 2: Telemedicine Patient Portal (Web)
- **Duration:** 8 Dec 2026 – 7 Jan 2027
- **Focus:** Accessible, web-based healthcare dashboard for elderly & general patients (Consultation booking, Video calls, Prescriptions).
- **Compliance:** WCAG 2.1 AA standards, calming healthcare palette, progressive disclosure booking flow.

---

## 🗂️ Repository Structure

```
Axlero/
├── research/              # Personas, IA maps, competitor notes, journey maps (.md)
│   └── .gitkeep
├── design-tokens/         # Color variables, typography scale, spacing tokens (JSON/CSS)
│   └── .gitkeep
├── icons/                 # Exported SVG icon assets
│   └── .gitkeep
├── figma-versions/        # Figma Named Version logs & milestone checkpoints
│   ├── .gitkeep
│   └── versions.md
└── README.md              # Project documentation & team roadmap
```

---

## 🎨 Figma File Architecture

Our Figma project adheres to the mandated 7-page standard structure:
1. `01_Cover` - Project thumbnail, metadata, team roles, and status (WIP/Review/Final).
2. `02_Research & Flows` - User personas, customer journey maps, and Information Architecture.
3. `03_Wireframes` - Low-fidelity grayscale structural layouts (no raw imagery).
4. `04_Design System` - Colors, typography, 8pt spacing grid, and reusable Auto-Layout components.
5. `05_High-Fidelity UI` - Pixel-perfect polished screens organized by user flow.
6. `06_Prototype` - Interactive clickable screens linked with Smart Animate.
7. `07_Developer Handoff` - Spacing redlines, design specs, interaction behaviors, and export assets.

🔗 **Figma Project File:** [Figma Workspace Link](https://figma.com) *(Update with team file link)*

---

## 🔄 Daily Commit Rota

To ensure compliance with Axlero's mandatory daily commit rule (no gaps allowed in the 20-day pre-review window):

| Day | Primary Owner | Backup Owner | Cutoff Time |
| :--- | :--- | :--- | :--- |
| **Monday** | Sudheer | Arnav | 9:00 PM IST |
| **Tuesday** | Shashank | Sudheer | 9:00 PM IST |
| **Wednesday** | Sajjad | Shashank | 9:00 PM IST |
| **Thursday** | Mukuture | Sajjad | 9:00 PM IST |
| **Friday** | Arnav | Mukuture | 9:00 PM IST |
| **Saturday** | Sudheer | Shashank | 9:00 PM IST |
| **Sunday** | Shashank | Arnav | 9:00 PM IST |

> **Lead Check:** Arnav verifies daily commits every night and manages PR merges into `main`.

---

## 🚀 Branching & Workflow Guidelines

1. **Clone & Switch Branch:**
   ```bash
   git clone https://github.com/arnavarya001/Axlero.git
   cd Axlero
   git checkout <your-branch-name>
   ```
2. **Daily Contribution:**
   ```bash
   git add .
   git commit -m "Add [feature/notes/assets description]"
   git push origin <your-branch-name>
   ```
3. **Pull Requests:** Individual branches are merged into `main` every 2–3 days by the Team Lead.

