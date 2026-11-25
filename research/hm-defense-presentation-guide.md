# Hiring Manager (HM) Design Presentation & Defense Guide

> **Project:** gather. (Multi-Vendor Marketplace App)  
> **Team Lead:** Arnav Arya (Group 1)  
> **Evaluation Phase:** Mid-Review & Design Defense  
> **Reference:** Axlero PRD Section 4 (Page 8)

---

## 🏛️ Pillar 1: UX Rationale & Cognitive Psychology

### 1. Why the "Terracotta & Canvas" Aesthetic?
* **Problem with standard e-commerce:** Most marketplaces look sterile, clinical, or overly corporate (aggressive blues, pure black `#000000`, stark white `#FFFFFF`).
* **Our Solution:** *gather.* is a marketplace for artisanal makers and handcrafted goods. We engineered a warm, grounded palette:
  * **Primary (`#A64028` - Terracotta):** Evokes earth, clay pottery, warmth, and deliberate craft without the aggressive urgency of bright discount reds. Passes WCAG AA contrast (`5.1:1`) on Canvas.
  * **Canvas (`#F7F4EF`):** Soft organic off-white that reduces eye strain during prolonged mobile browsing compared to raw white.
  * **Ink (`#222820`):** Softened deep charcoal that prevents optical glare and maintains high legibility (`13.2:1`).

### 2. Defending the 3-Screen Checkout Flow
* **Industry Pain Point:** Standard e-commerce averages 5 to 7 screens (Cart ➔ Address ➔ Delivery Slot ➔ Merchant Selection ➔ Coupon Code ➔ Payment Gateway ➔ OTP ➔ Confirmation), causing massive cart abandonment (upwards of 68%).
* **Our Architecture:**
  1. **Screen 1 (Address & Consolidated Shipping):** Groups items from multiple independent vendors into one consolidated delivery window.
  2. **Screen 2 (Payment & Verification):** One-tap modern digital wallets (UPI, Apple Pay) with upfront itemized totals (zero hidden surprise fees).
  3. **Screen 3 (Order Confirmed):** Immediate dopamine feedback with clear vendor dispatch timelines and trackable order IDs.

---

## 🏗️ Pillar 2: System Architecture & Component Engineering

### 1. Auto-Layout and Responsive Constraints
* **100% Auto-Layout Compliance:** Every single screen frame and component uses vertical/horizontal flex containers with fixed padding and `Fill container` constraints.
* **Spatial System:** Rigid adherence to an **8pt Grid** (`4px`, `8px`, `16px`, `24px`, `32px`, `48px`). No arbitrary margin or padding values exist anywhere in the canvas.
* **Component Variants & Properties:** Buttons and form inputs utilize Figma Boolean properties and component variants (Default, Hover, Active, Disabled).

### 2. Two-Sided Platform Architecture
* Designed both the **Consumer App** (Discovery, Search, PDP, 3-Screen Checkout) and the **Vendor Dashboard** (Live revenue KPIs, order dispatch queue, and a 4-step mobile listing workflow).

---

## 🔄 Pillar 3: Workflow Maturity & Version Control

### 1. Defending the 3-Page Figma Free Tier Architecture
* **The Constraint:** Figma Starter (Free) plan limits files to 3 pages, whereas the Axlero PRD requests 7 page titles.
* **The Engineering Decision:** Rather than leaving loose files or cutting content, we built a **Consolidated 3-Page Architecture**:
  * `01-04 · Foundations` (Cover, Research/Flows, Wireframes, UI Kit)
  * `05 · High-Fidelity UI` (Complete Consumer & Vendor flows)
  * `06-07 · Prototype & Handoff` (Interactive flows & Developer Handoff)
* **The Documentation:** Formally mapped in `figma-versions/Figma_3Page_Architecture_Guide.md` and linked in `README.md`.

### 2. Audit Trail & Version Control Discipline
* Weekly Named Versions saved in Figma (`[Week 1] UX & Wireframes`, `[Week 2] Design System`, `[Week 3] Hi-Fi Screens`, `[Week 4] Prototype & Spec`).
* GitHub repository maintained with daily markdown logs, JSON/CSS token exports, and SVG icon libraries.
