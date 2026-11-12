# Wireframe Specifications & Layout Briefs
## Project 1: Multi-Vendor Marketplace App (Mobile)

> **Design Rules for All Wireframes:**
> 1. **Frame Dimensions:** `390px × 844px` (iPhone 14 standard) or `360px × 800px` (Android).
> 2. **Grayscale Only:** Strict adherence to grayscale palette (`#FFFFFF`, `#F5F5F5`, `#E0E0E0`, `#9E9E9E`, `#212121`). No colored accents.
> 3. **Image Placeholders:** Box with an `X` across it or a simple gray mountain icon container.
> 4. **Auto-Layout:** Every screen must be wrapped in a vertical Auto-Layout container with 8pt spacing system (`8px`, `16px`, `24px`, `32px`).
> 5. **Target Figma Page:** Place all low-fidelity frames in `03_Wireframes`.

---

## 📱 Consumer App Screens

### 1. Home Screen (Assigned to: Sajjad)
*User goal: Discover products, browse categories, see active vendor promotions.*

* **Header / Top Bar (Fixed, H: 64px):**
  - Left: Location selector (`Deliver to: 110001 ▼`)
  - Right: Notification bell icon + Wishlist heart icon
* **Search Bar Container (H: 48px, Margin: 16px):**
  - Search icon + placeholder text: *"Search 10,000+ products across local sellers..."*
  - Right: Voice mic icon + camera search icon
* **Promotional Banner Carousel (H: 160px):**
  - Large gray placeholder box (`[X]`) with dot indicators (`● ○ ○ ○`) below it.
* **Category Icon Grid (H: ~180px):**
  - 2 rows × 4 columns of circular containers (`56px × 56px`) with 1-line label underneath (Electronics, Fashion, Home, Grocery, Beauty, Sports, Books, More).
* **Vendor Spotlight Carousel (H: 120px):**
  - Section header: *"Verified Local Sellers"* + *"View All"* link.
  - Horizontal scroll cards: Seller logo avatar (`40px`), Store name, Star rating badge (`★ 4.8`), Badge: `"Verified"`.
* **Featured / Flash Deals Grid (2-Column):**
  - Section header: *"Deals of the Day"* + Countdown timer badge (`[ 04h : 22m : 15s ]`).
  - 2-Column Product Cards (`170px × 240px`):
    - Top: Image box (`170px × 140px`) with wishlist heart icon button top-right.
    - Vendor name (small 12px text).
    - Product title (2-line truncation).
    - Price line: Discounted price (`$24`) + Strikethrough price (`$35`) + Discount pill (`-30%`).
    - Bottom button: `+ Add` button.
* **Bottom Navigation Bar (Fixed, H: 64px):**
  - 5 Icons: `Home` (Active), `Categories`, `Deals`, `Cart (badge: 2)`, `Account`.

---

### 2. Category Search & Filter Screen (Assigned to: Sajjad)
*User goal: Filter and compare multi-vendor products with ease.*

* **Header Bar (H: 56px):**
  - Back arrow `←` + Search input field (with clear `✕` button) + Filter button.
* **Horizontal Filter Chips (Scrollable, H: 40px):**
  - Chips: `All`, `Price: Low to High ▼`, `Rating 4.0+`, `Fast Delivery`, `Brand ▼`, `Vendor Rating ▼`.
* **Results Metadata & Sort Bar (H: 36px):**
  - Left: *"Showing 248 items"*
  - Right: Sort dropdown (`Relevance ▼`) + View toggle (Grid / List).
* **Product Grid (2 Columns, Infinite Scroll):**
  - Repeated Product Card components.
  - Multi-vendor differentiator: Highlight vendor name in a small pill badge (`By: Urban Store`).
* **Active Filter Modal / Bottom Sheet (Triggered by Filter button):**
  - Price Range Slider (`$10 - $500`).
  - Checkboxes for Category, Seller Ratings (`4★ & above`), and Delivery Time (`Same Day`, `2-Day`).
  - Sticky bottom action buttons: `Clear All` (Secondary text) and `Apply Filters` (Primary full-width).

---

### 3. Product Detail Page — PDP (Assigned to: Mukuture)
*User goal: Inspect product specs, choose variants, check seller reputation, and purchase.*

* **Top Bar (Transparent / Fixed on scroll, H: 56px):**
  - Left: Back button `←`
  - Right: Share button + Wishlist heart toggle + Cart icon with badge counter.
* **Product Image Gallery (H: 340px):**
  - Full-width image carousel placeholder with pagination dots (`1 / 5`).
* **Product Identification & Pricing Container:**
  - Brand name / Vendor link (`Sold by: Apex Retailers ★ 4.9 (1.2k reviews)`).
  - Product Title (Bold, 20px, 2-3 lines).
  - Rating badge (`4.7 ★`) + *"342 reviews"*.
  - Price block: Bold current price, MRP with strikethrough, savings pill.
* **Variant Selectors:**
  - Color selector: Color swatches (grayscale circles with outline for selected).
  - Size / Model selector: Segmented pill buttons (`S`, `M`, `L`, `XL`, `XXL`).
* **Delivery & Seller Trust Info Card:**
  - Pincode check box with `Check` button.
  - Trust bullets: `✓ 7-Day Replacement`, `✓ Free Delivery`, `✓ Secure Payment`.
* **Expandable Product Details (Accordion):**
  - `Description` ▼
  - `Specifications` ▼
  - `Customer Reviews & Q&A` ▼
* **Sticky Bottom Action Bar (Fixed, H: 72px):**
  - Left: Quantity Stepper (`[-]  1  [+]`)
  - Middle: `Add to Cart` (Outlined / Secondary button)
  - Right: `Buy Now` (Solid / Primary button)

---

### 4. Cart Screen (Assigned to: Mukuture)
*User goal: Review selected items, adjust quantities, apply coupons, and start checkout.*

* **Header (H: 56px):**
  - Back arrow `←` + Title: *"My Cart (3 Items)"*
* **Delivery Address Preview Strip (H: 44px):**
  - Pin icon + *"Deliver to Home - 123 Baker St..."* + *"Change"* link.
* **Cart Items List (Grouped by Vendor):**
  - Vendor Header: Store icon + *"Store: TechHub India"*
  - Cart Item Row (`100px` height):
    - Thumbnail image (`70px × 70px`)
    - Title, selected variant pill (`Size: M`)
    - Unit price (`$45.00`)
    - Quantity Stepper (`[-]  1  [+]`) + Trash / Remove icon.
* **Coupons & Promo Card:**
  - Input field: `Enter Coupon Code` + `Apply` button.
* **Bill Details / Order Summary Card:**
  - Item Total: `$135.00`
  - Delivery Fee: `Free`
  - Taxes: `$12.00`
  - Coupon Discount: `-$15.00`
  - **Total Amount Payable:** **`$132.00`**
* **Sticky Bottom Bar:**
  - Left: Total Price display (`$132.00`)
  - Right: Primary full-width CTA: `Proceed to Checkout (3) →`

---

### 5. Checkout Flow (Assigned to: Arnav Arya)
*Mandatory Rule: Maximum 3 screens from "Add to Cart" to "Order Confirmed".*

#### Screen 5A: Shipping & Address (Step 1 of 3)
* **Progress Stepper Header (H: 40px):** `[1. Address] ─── (2. Payment) ─── (3. Confirm)`
* **Saved Addresses Radio Group:**
  - Radio Card 1 (Selected): Home address (Name, phone, street, city, pin).
  - Radio Card 2: Office address.
  - `+ Add New Address` dashed border card button.
* **Delivery Speed Selector:**
  - Standard Delivery (3-5 days - Free) vs Express Delivery (Tomorrow - $5.00).
* **Sticky CTA:** `Continue to Payment →`

#### Screen 5B: Payment Options (Step 2 of 3)
* **Progress Stepper Header:** `(✓ Address) ─── [2. Payment] ─── (3. Confirm)`
* **Payment Methods Accordion:**
  - `UPI / QR Code` (GPay, PhonePe, Paytm)
  - `Credit / Debit Card` (Card number, expiry, CVV input fields)
  - `Net Banking` (Bank selector grid)
  - `Cash on Delivery (COD)` (with verification captcha box)
* **Order Summary Recap (Collapsible box):** Total items: 3, Payable: `$132.00`.
* **Sticky CTA:** `Pay & Place Order ($132.00) 🔒`

#### Screen 5C: Order Confirmation (Step 3 of 3)
* **Success Graphic:** Large checkmark illustration container (`[✓]`).
* **Headline:** *"Order Confirmed!"*
* **Order ID & Timestamp:** *"Order #AXL-98432 placed successfully."*
* **Delivery ETA Card:** Expected delivery date + Estimated tracking bar.
* **Action Buttons:**
  - Primary button: `Track Order`
  - Secondary button: `Continue Shopping`

---

## 🏢 Vendor Dashboard Screens

### 6. Vendor Sales Analytics (Assigned to: Sudheer)
*Screen Target: Mobile / Tablet responsive view.*

* **Vendor Header:** Store logo, store name (`Apex Store`), switch to consumer app toggle.
* **Key Metric Stat Cards (2 × 2 Grid):**
  - Card 1: Today's Revenue (`$1,420` +14%)
  - Card 2: Active Orders (`18 pending`)
  - Card 3: Units Sold (`86 items`)
  - Card 4: Store Rating (`4.8 ★`)
* **Sales Overview Chart Placeholder:**
  - Bar/Line chart box with Weekly/Monthly toggle chips.
* **Recent Orders Table / List:**
  - Order #, Customer name, Items, Amount, Status pill (`Processing`, `Shipped`, `Delivered`).

---

### 7. Add Product Form (Assigned to: Arnav Arya)
*User goal: Streamlined multi-step form for sellers to list new inventory.*

* **Image Uploader Container:** Dashed box with camera icon + *"Upload up to 6 high-res photos"*.
* **Product Basic Info:**
  - Input: Product Title
  - Dropdown: Category & Subcategory
  - Textarea: Description & Key Highlights
* **Pricing & Inventory:**
  - Input: Regular Price, Sale Price
  - Input: Available Stock (SKU Quantity)
* **Variants Setup:**
  - Add Variant button (`Color`, `Size`, `Material`).
* **Bottom Action:** `Save as Draft` (Secondary) + `Publish Product` (Primary).

