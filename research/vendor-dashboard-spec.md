# ShopVerse: Vendor Dashboard Architecture & Workflow Specifications
**Lead Designer:** Arnav Arya (Team Lead)  
**Assigned Domain:** Vendor Management & Merchant Portal Architecture  
**Focus Modules:** 1. Sales & Revenue Analytics  |  2. Multi-Step "Add Product" Workflow

---

## 1. System Context & Seller Pain Points
Multi-vendor marketplaces fail when seller tooling is clunky or requires a desktop computer. For **ShopVerse**, we engineered a **mobile-first merchant portal** allowing independent artisans, D2C brands, and local retailers to track orders, manage stock, and publish new SKUs straight from their smartphones.

---

## 2. Screen 1: Vendor Sales Analytics (`390px × 844px`)

### A. Merchant Header Bar
- Merchant Branding: Store Logo Avatar (`44px × 44px`), Store Name (*"Apex Leathercraft"*), Verification Badge (`✓ Verified Merchant`).
- Switcher Control: One-tap toggle: `[Merchant Portal] ⇄ [Consumer View]`.
- Notification Bell with unread orders badge (`🔴 4`).

### B. KPI Stat Cards (2 × 2 Auto-Layout Grid)
1. **Net Revenue Card:**
   - Value: **₹1,42,850**
   - Trend Indicator: `▲ +18.4% vs last week` (in `#35664D` green).
2. **Orders Volume Card:**
   - Value: **128 Orders**
   - Breakdown: `12 Pending Dispatch` | `116 Delivered`.
3. **Average Order Value (AOV):**
   - Value: **₹1,116**
   - Trend: `▲ +4.2%`.
4. **Merchant Store Rating:**
   - Value: **4.85 ★** (Based on 342 customer reviews).

### C. Visual Revenue Chart Placeholder
- Segmented filter chips: `[Today] [This Week] [This Month] [Custom]`.
- Clean bar graph showing hourly/daily sales volume with peak transaction markers.

### D. Real-Time Order Management Queue
- Filter Tabs: `[All (128)]` `[Pending (12)]` `[In Transit (34)]` `[Completed (82)]`.
- Order Item Card:
  - Order `#ORD-8821` • ₹2,499 • 2 items.
  - Customer: Priya S. (Bengaluru).
  - Quick action buttons: `Generate Shipping Label` | `Mark as Ready for Pickup`.

---

## 3. Screen 2: Add Product Workflow (Multi-Step Form)

### Step 1: Media & Imagery
- Drag-and-drop / Camera tap container (`H: 180px` with dashed border `#DED9D1`).
- Supported formats: JPEG, PNG, WEBP (Max 5MB each).
- Primary image selector + 5 thumbnail slots with delete (`✕`) badges.

### Step 2: Product Categorization & Identification
- Product Title Input (Max 80 characters): Auto-validates against keyword stuffing.
- Category Hierarchy Selector:
  - Primary Category: `Fashion & Accessories`
  - Subcategory: `Bags & Backpacks`
  - Item Type: `Leather Laptop Messenger Bag`
- Brand / Maker Tag.

### Step 3: Pricing, Inventory & Variants
- Regular Selling Price (₹) & MRP (₹) ➔ Auto-calculates customer discount % pill.
- GST Slab Selector: `[0%] [5%] [12%] [18%]`.
- SKU Quantity Stepper: In-stock units counter with low-stock threshold alert setting.
- Variant Generator:
  - Add Attribute: `Color` (Tan, Black, Olive) + `Size` (14-inch, 16-inch).
  - Dynamically builds inventory matrix for each combination.

### Step 4: Shipping Specs & Dimensions
- Weight in grams (`kg/g`).
- Package Dimensions (`L × W × H in cm`) for automated courier rate estimation.

### Fixed Action Footer:
- Left: `Save as Draft` (Secondary outlined button).
- Right: `Publish to ShopVerse Live 🚀` (Primary solid brand button `#A64028`).

---
*Authored by Arnav Arya — Team Lead, Axlero UI/UX Group 1.*
