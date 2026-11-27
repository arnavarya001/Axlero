# Edge Cases, Error States & Usability Architecture

> **Project:** gather. (Multi-Vendor Marketplace App)  
> **Design Sprint:** Week 3 / Week 4 Resilience Architecture  
> **Reference:** Axlero PRD Week 4 (Edge Cases & Final Usability)

---

## 🛡️ 1. Multi-Vendor Edge Cases & Solutions

### Edge Case A: Partial Vendor Stock Depletion
* **Scenario:** A buyer has added products from Seller A (Jaipur Crafts) and Seller B (Earthen Roots). While in checkout, Seller B's item runs out of stock.
* **UX Solution:**
  * Avoid discarding the entire cart.
  * Display a non-blocking informational modal: *"Linen Throw from Earthen Roots just sold out. We have moved it to your Saved items."*
  * Automatically recalculate total payable for Seller A's item without resetting user shipping address.

### Edge Case B: Asynchronous Vendor Dispatch Timelines
* **Scenario:** Items ordered together will arrive on different dates because independent artisans operate from distinct locations.
* **UX Solution:**
  * Screen 1 of Checkout displays a grouped breakdown:
    * `Package 1 (Jaipur Crafts): Estimated delivery 28 Nov`
    * `Package 2 (Earthen Roots): Estimated delivery 30 Nov`
  * Single payment transaction covers both packages with clear per-package tracking links upon confirmation.

---

## ⚠️ 2. Empty States Architecture

### 1. Empty Cart State
* **Visual:** Minimalist terracotta line illustration of an open wicker basket.
* **Headline:** *"Your basket is currently empty"*
* **Subtext:** *"Discover meaningful handcrafted goods from local independent makers."*
* **Primary Action CTA:** `Explore Artisans →` (Deep-links to Home Discovery feed).

### 2. Search Zero Results State
* **Visual:** Magnifying glass with an organic leaf motif.
* **Headline:** *"No direct finds for '[User Query]'"*
* **Corrective Guidance:**
  * Check spelling or try broader terms (e.g., `Ceramics`, `Linen`, `Decor`).
  * Display horizontal carousel of *"Trending Makers"* so user never hits a dead-end screen.

---

## ⚡ 3. Network Failure & Payment Recovery

### Offline / Connectivity Drop
* **Trigger:** Network disconnects while buyer clicks "Confirm Order".
* **Behavior:**
  * Persistent offline indicator banner: *"You are offline. We will resume your transaction once connected."*
  * Cache form inputs in local storage (`AsyncStorage` / `UserDefaults`) to prevent data loss.
  * Idempotency token passed with payment request to ensure duplicate charges never occur upon reconnection.
