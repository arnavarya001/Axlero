# ShopVerse: 3-Screen Checkout UX Architecture & Flow Specification
**Lead Designer:** Arnav Arya (Team Lead)  
**Assigned Domain:** Checkout Optimization & Conversion Architecture  
**Target Metric:** Strict Maximum of 3 Screens from "Add to Cart" to "Order Confirmed" (Axlero PRD Metric)

---

## 1. Executive Summary & Design Rationale
In modern multi-vendor e-commerce applications, checkout friction accounts for up to 68% of cart abandonment. Traditional desktop flows force users through 5 to 7 separate pages (Login ➔ Cart ➔ Shipping ➔ Billing ➔ Shipping Method ➔ Payment Review ➔ Confirmation). 

For **ShopVerse**, we consolidate the flow into a **frictionless 3-step progressive disclosure architecture** optimized for 390 × 844 mobile viewports:

```
[Screen 1: Shipping & Delivery] ──► [Screen 2: Payment & Review] ──► [Screen 3: Order Confirmed]
```

---

## 2. Detailed Screen Breakdown

### Screen 1: Shipping & Delivery Selection (`390px × 844px`)
*Objective: Collect recipient address and delivery urgency with zero friction.*

* **Header Navigation (Fixed H: 56px):**
  - Left: Back button (`←`) returning to Cart.
  - Center: Stepper Indicator: `[Step 1 of 3: Delivery]` (Visual progress bar at 33%).
  - Right: Security Badge (Lock icon: *"256-bit SSL Secure"*).
* **Delivery Address Selector:**
  - Active Radio Card (Default):
    - Recipient: Arnav Arya (+91 98765-43210)
    - Address: Flat 402, Green Glen Layout, Bellandur, Bengaluru, Karnataka - 560103.
    - Tag: `[Home - Default]`
    - Action: *"Edit"* button.
  - Secondary Radio Card: `[Work]` address.
  - Dashed Action Card: `+ Add New Delivery Address` (Triggers bottom drawer).
* **Delivery Preference Options:**
  - Standard Delivery (3–4 business days) — **FREE**
  - Express Priority Delivery (Next Day before 2 PM) — **₹99**
* **Sticky Bottom Checkout Bar (H: 72px):**
  - Total: **₹1,499** (Includes taxes & free delivery)
  - CTA Button: `Proceed to Payment →` (Full width, Height: 44px, Background: `#A64028`).

---

### Screen 2: Payment Gateway & Order Review (`390px × 844px`)
*Objective: Seamless payment selection with instant total verification.*

* **Header Navigation:**
  - Stepper Indicator: `[Step 2 of 3: Payment]` (Progress bar at 66%).
  - Back button (`←`) returning to Screen 1.
* **Payment Methods Accordion:**
  - **Option A: Instant UPI / QR (Recommended):**
    - Quick App Intent buttons: Google Pay, PhonePe, Paytm, BHIM.
    - UPI ID input field (`username@bank`) with real-time verify button.
  - **Option B: Credit / Debit Cards:**
    - Card Number input (Luhn-checked with auto-detected Visa/Mastercard/RuPay logos).
    - Expiry Date (`MM/YY`) & CVV (`3 digits`) with tooltip explanation.
    - Secure card tokenization checkbox (RBI compliant).
  - **Option C: Net Banking:**
    - Top 6 Indian Banks quick-select grid + searchable dropdown for all banks.
  - **Option D: Cash on Delivery (COD):**
    - Security Captcha input verification to minimize fake/spam orders.
* **Order Summary Recap Card (Collapsible):**
  - Vendor 1 items (2 products) + Vendor 2 items (1 product).
  - Subtotal: ₹1,699 | Discount: -₹200 | Delivery: ₹0
  - **Net Payable: ₹1,499**
* **Sticky Bottom Payment Button:**
  - CTA Button: `Pay ₹1,499 & Place Order 🔒` (Auto-displays selected payment icon).

---

### Screen 3: Order Confirmation & Live Tracking (`390px × 844px`)
*Objective: Immediate cognitive relief, order verification, and vendor dispatch timeline.*

* **Hero Success Section (H: 260px):**
  - Animated Success Checkmark (`#35664D`).
  - Headline: *"Thank You, Arnav! Your Order is Confirmed."*
  - Order Reference: `#SV-2026-89412` (with one-tap Copy icon).
* **Delivery Timeline Card (Auto-Layout):**
  - Dynamic Progress Tracker:
    - `[✓] Order Placed (Today, 18 Nov)`
    - `[ ] Dispatched by Vendors (19 Nov)`
    - `[ ] Out for Delivery (21 Nov)`
    - `[ ] Expected Delivery (22 Nov)`
* **Vendor Multi-Shipment Notice:**
  - Alert Card (`#EEF1FB`): *"Items will arrive in 2 separate eco-friendly packages from Apex Stores & TechHub."*
* **Post-Purchase Actions:**
  - Primary CTA: `Track Shipment Details`
  - Secondary CTA: `Continue Shopping`
  - Small text link: *"Download Tax Invoice (PDF)"*

---

## 3. WCAG AA Contrast Compliance
All text elements on payment and address forms strictly adhere to WCAG 2.1 AA standards:
- `#A64028` on `#FFFFFF` ➔ Contrast Ratio **4.85:1** (Passes AA for normal text).
- `#222820` on `#F7F4EF` ➔ Contrast Ratio **12.6:1** (Passes AAA).
- `#35664D` (Success) on `#FFFFFF` ➔ Contrast Ratio **5.2:1** (Passes AA).

---
*Authored by Arnav Arya — Team Lead, Axlero UI/UX Group 1.*
