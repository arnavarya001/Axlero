# Interactive Prototype & Micro-Interactions Specification

> **Workspace Canvas:** `06-07 · Prototype & Handoff`  
> **Target Device Viewport:** iPhone 14 (`390 × 844 px`)  
> **Easing Formula:** `Ease Out` / `Smart Animate` (Smooth 250ms – 350ms curves)

---

## ⚡ Core Prototype Interaction Flows

```
[Home Feed] ──(Tap Search)──> [Search & Filters]
     │
     └──(Tap Product Card)──> [Product Detail Page] ──(Tap Buy Now)──> [3-Screen Checkout]
                                      │                                      │
                               (Tap + Add to Cart)                           ├── Step 1: Address
                                      │                                      ├── Step 2: Payment
                               [Toast & Cart Badge +1]                       └── Step 3: Confirmation
```

---

## 🎬 Micro-Interaction Matrix

| User Trigger | Source Frame | Destination Frame | Transition Type | Duration & Curve | UX Intent |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Tap Search Bar** | `Home` | `Search · Home & living` | Push Left | `300ms`, Ease-Out | Communicates spatial drill-down into category discovery. |
| **Tap Category Chip** | `Search` | `Search (Filtered)` | Smart Animate | `200ms`, Ease-In-Out | Instant visual feedback with smooth badge highlight. |
| **Tap Product Card** | `Home` / `Search` | `Product · Everyday mug` | Smart Animate (Hero Image) | `350ms`, Gentle | Shared element transition for smooth visual continuity. |
| **Tap Variant (Size/Color)** | `Product Detail` | `Product Detail (Active)` | Instant / Highlight | `150ms`, Linear | Clear tactile confirmation of selected SKU. |
| **Tap "+ Add to Cart"** | `Product Detail` | Sticky Toast Bar | Smart Animate (Slide Up) | `250ms`, Ease-Out | Reassures buyer that item is added without leaving page. |
| **Tap "Proceed to Pay"** | `Checkout (Step 1)` | `Checkout (Step 2)` | Slide Left | `300ms`, Ease-Out | Step progression through the 3-screen checkout flow. |
| **Tap "Confirm Order"** | `Checkout (Step 2)` | `Order Confirmed` | Smart Animate (Checkmark) | `400ms`, Bouncy | Dopamine payoff: Animated checkmark and green success badge. |

---

## 🏢 Vendor Dashboard Interactions

| Action | Transition | Behavior |
| :--- | :--- | :--- |
| **KPI Card Tab** | Instant Filter | Switches between "Today's Sales", "Orders Pending", and "Stock Warnings". |
| **Add Product Wizard** | Step Slide (`1 ➔ 2 ➔ 3 ➔ 4`) | 4-step progress bar smoothly increments from 25% to 100%. |
