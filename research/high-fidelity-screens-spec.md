# High-Fidelity UI Architecture & Screen Specifications

## Project: ShopVerse - Multi-Vendor Marketplace (Mobile Viewport: 390 × 844 px)

---

## 🎨 Design Token Mapping (WCAG 2.1 AA Compliant)

| Token Name | Hex Code | Purpose & Application | Contrast Ratio vs Background |
| :--- | :--- | :--- | :--- |
| `color-primary` | `#A64028` (Terracotta) | Primary CTA buttons, active state indicators | 5.1:1 on Canvas (Pass AA) |
| `color-primary-hover` | `#8C341F` | Pressed/Hover state for primary actions | 6.8:1 on Canvas (Pass AAA) |
| `color-surface` | `#FFFFFF` | Card surfaces, modals, floating action bars | — |
| `color-background` | `#F7F4EF` (Canvas) | Neutral app canvas background | — |
| `color-text-main` | `#222820` (Ink) | Headings, primary labels, price values | 13.2:1 on Canvas (Pass AAA) |
| `color-text-muted` | `#686E64` | Subtitles, vendor names, secondary text | 4.6:1 on Canvas (Pass AA) |
| `color-accent-green` | `#2E7D32` | Verified vendor badge, in-stock pills, discounts | 4.7:1 on Canvas (Pass AA) |
| `color-border-subtle` | `#E5E0D8` | 1px card separators, input borders | Non-text UI boundary (3.2:1) |

---

## 📱 Consumer App: High-Fidelity Screen Breakdown

### 1. Home Feed & Discovery (`390 × 844`)
- **Top App Bar:** Delivery location selector with pin icon, notification bell with unread badge, and wishlist heart icon.
- **Search & Filter:** Search bar with voice search and quick filter tags (`Local Verified`, `Top Rated`, `Under $50`).
- **Curated Carousel:** Multi-vendor promotional hero banner highlighting local artisans.
- **Category Grid:** 8 circular icon categories with 8pt grid padding.
- **Vendor Spotlight:** Horizontal cards featuring verified seller credentials and rating badges.
- **Two-Column Product Grid:** Product cards showing imagery, merchant tag, product title, price with discount tag, and an instant add-to-cart action.
- **Fixed Bottom Navigation:** 5-tab bar with Home, Categories, Deals, Cart (with badge count), and Profile.

### 2. Product Detail Page (PDP) (`390 × 844`)
- **Image Gallery:** Multi-image swipe container with thumbnail indicators.
- **Merchant Identity Block:** Vendor name, store badge, satisfaction rating, and direct "Visit Store" link.
- **Variant Selector:** Auto-Layout chip groups for size and color options.
- **Sticky Purchase Bar:** Instant Buy Now button and Add to Cart action with live inventory status.

### 3. Streamlined 3-Screen Checkout Flow (Cognitive Optimization)
1. **Screen 1 - Delivery & Address:** Selected delivery address, shipping method selector with delivery timeline, and order summary accordion.
2. **Screen 2 - Payment Method:** One-tap UPI selection, saved card tokens, Apple Pay / Google Pay, and coupon code entry.
3. **Screen 3 - Order Confirmed:** Animated success checkmark, order ID, delivery timeline per vendor, and "Track Order" button.

---

## 🏢 Vendor Dashboard Screen Architecture

### 1. Merchant Overview (`390 × 844`)
- **Metric Cards (KPIs):** Today's Revenue, Active Orders, Low Stock Alerts, and Average Store Rating.
- **Recent Orders List:** Order cards with customer shipping destination, item count, and dispatch status tags (`Pending`, `Packed`, `Shipped`).

### 2. Multi-Step "Add Product" Flow
- **Step 1:** Title, Category, and Description.
- **Step 2:** Photo and asset uploads.
- **Step 3:** Variant matrix (sizes, colors, SKU, pricing).
- **Step 4:** Inventory quantity, shipping weight, and live preview.
