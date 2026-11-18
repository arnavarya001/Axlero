# ShopVerse: Navigation Components & 8pt Spacing System
**Lead Designer:** Arnav Arya (Team Lead)  
**Assigned Deliverable:** Global Navigation Components & Layout Grid Standards (Week 2 UI Kit)

---

## 1. 8pt Spatial Grid Standard

In strict accordance with the Axlero UI/UX Directives, all margins, paddings, gutters, and component dimensions adhere to the **8pt grid system** (with a 4pt half-step for micro-elements):

| Token Name | Value | Recommended Usage |
|:---|:---:|:---|
| `space-xxs` | `4px` | Icon-to-text micro gap, badge inner padding, border radiuses |
| `space-xs` | `8px` | Inner button padding, inline element spacing |
| `space-sm` | `12px` | Card internal content gaps |
| `space-md` | `16px` | Standard screen edge margin (Left/Right gutters for 390px viewports) |
| `space-lg` | `24px` | Section vertical rhythm between distinct content blocks |
| `space-xl` | `32px` | Major group separation on Home and PDP |
| `space-xxl` | `40px` | Hero banner padding and modal top clearance |
| `space-xxxl` | `48px` | Minimum touch-target height for interactive CTA buttons |

---

## 2. Top Navigation Bar Component Specification

### Standard Consumer Top Bar (`H: 64px, W: 390px`)
- **Container Styling:**
  - Background: `#F7F4EF` (Canvas) or `#FFFFFF` (Surface when scrolled).
  - Bottom Stroke: `1px solid #DED9D1` on scroll trigger.
  - Padding: `12px 16px`.
- **Sub-Components (Auto-Layout Horizontal, Space Between):**
  1. **Delivery Location Selector (Left):**
     - Icon: Location Pin (`18px × 18px`, `#A64028`).
     - Text container (Vertical):
       - Label: *"Deliver to"* (`9px`, `#68716B`, uppercase).
       - Value: *"Bengaluru 560103 ▼"* (`12px`, `#222820`, SemiBold).
  2. **Utility Action Icons (Right):**
     - Wishlist Heart (`24px × 24px`, `#222820`) with hover highlight.
     - Notification Bell (`24px × 24px`) with unread badge counter (`#A64028`, dot size `8px`).

---

## 3. Bottom Tab Bar Component Specification

### Global Consumer Tab Bar (`H: 64px, W: 390px, Fixed`)
- **Container Styling:**
  - Background: `#FFFFFF` (Solid surface).
  - Top Stroke: `1px solid #DED9D1`.
  - Elevation / Shadow: `0px -2px 10px rgba(34, 40, 32, 0.05)`.
  - Layout: 5 equal columns (`78px` width each).
- **Tab Items:**
  1. **Home:** Icon `⌂` (`22px`), Label *"Home"* (`10px`).
     - *Active State:* Icon & Label in `#A64028` (Brand Primary) with active top indicator pill (`W: 24px, H: 2px`).
  2. **Categories:** Icon `⌕` (`22px`), Label *"Explore"* (`10px`).
     - *Inactive State:* `#68716B` (Muted Ink).
  3. **Deals:** Icon `🏷` (`22px`), Label *"Offers"* (`10px`).
  4. **Cart:** Icon `▢` (`22px`), Label *"Cart"* (`10px`).
     - *Badge:* Dynamic red pill counter (`H: 16px, Min-W: 16px`, `#A64028`, White 9px bold text).
  5. **Profile:** Icon `👤` (`22px`), Label *"Account"* (`10px`).

---
*Authored by Arnav Arya — Team Lead, Axlero UI/UX Group 1.*
