# Information Architecture (IA) & Category Taxonomy Specification

> **Project:** gather. (Multi-Vendor Marketplace App)  
> **Mobile Standard:** iOS (`390 × 844 pt`) & Android (`360 × 800 dp`)  
> **Author:** Arnav Arya (Team Lead, Group 1)  
> **Date:** 28 November 2026

---

## 🗺️ 1. App-Wide Navigation Hierarchy Tree

```
Root: gather. Mobile App
│
├── 1.0 Home / Discovery Tab (Active)
│   ├── 1.1 Curated Hero Banner (Artisan of the Month)
│   ├── 1.2 Quick Category Circles (8 Core Categories)
│   ├── 1.3 Verified Vendor Spotlight (Horizontal Carousel)
│   ├── 1.4 Trending Handcrafted Goods (2-Column Grid)
│   └── 1.5 Notification Center & Delivery Location Selector
│
├── 2.0 Explore / Search Tab
│   ├── 2.1 Keyword & Voice Search Bar
│   ├── 2.2 Filter Chips (Price, Rating, Fast Delivery, Craft Type)
│   ├── 2.3 Category Taxonomy Drilldown
│   └── 2.4 Multi-Attribute Filter Modal (Drawer)
│
├── 3.0 Saved / Wishlist Tab
│   ├── 3.1 Saved Products Grid
│   └── 3.2 Followed Artisan Workshops
│
├── 4.0 Cart & Checkout Flow (Optimized 3-Screen Architecture)
│   ├── 4.1 Multi-Vendor Cart Drawer (Grouped by Artisan)
│   ├── 4.2 Step 1: Address & Consolidated Shipping Method
│   ├── 4.3 Step 2: Payment Method (UPI, Apple Pay, Cards)
│   └── 4.4 Step 3: Order Confirmed & Multi-Package Dispatch Tracking
│
└── 5.0 Account & Vendor Portal Tab
    ├── 5.1 Buyer Profile & Order History
    ├── 5.2 Saved Shipping Addresses & Payment Tokens
    └── 5.3 Switch to Vendor Dashboard (Merchant Mode)
        ├── 5.3.1 Sales Analytics & Revenue KPIs
        ├── 5.3.2 Customer Orders Queue (Dispatch Management)
        └── 5.3.3 4-Step "Add Product" Wizard
```

---

## 🏷️ 2. Artisanal Category Taxonomy (8 Core Categories)

| # | Core Category | Sub-Categories (Taxonomy Nodes) | Target Artisan Niche |
| :---: | :--- | :--- | :--- |
| **1** | **Pottery & Ceramics** | Mugs & Cups, Vases & Planters, Tableware, Sculptural Pieces | Studio potters, stoneware makers |
| **2** | **Textiles & Linens** | Handwoven Throws, Pure Linen Bedding, Rugs & Dhurries, Cushion Covers | Heritage looms, natural fiber weavers |
| **3** | **Living & Decor** | Brass & Copper Ware, Wooden Artifacts, Candle Holders, Wall Art | Metalworkers, woodturners |
| **4** | **Leather & Goods** | Journals & Folios, Cardholders & Wallets, Bags, Belts | Vegetable-tanned leather crafters |
| **5** | **Slow Fashion** | Khadi & Organic Apparel, Hand-printed Scarves, Robes | Sustainable small-batch tailors |
| **6** | **Wellness & Scents** | Soy Wax Candles, Botanical Incense, Essential Oils, Bath Salts | Natural apothecary & candlemakers |
| **7** | **Paper & Stationery** | Handmade Cotton Rag Paper, Calligraphy Kits, Notebooks, Print Art | Heritage papermakers & illustrators |
| **8** | **Organic Pantry** | Single-Origin Honey, Artisanal Teas, Cold-Pressed Oils, Spices | Small organic farm collectives |

---

## 🔗 3. Deep-Linking Schema & Routing Architecture

| Intent / Action | Mobile Deep-Link URI | Target Screen |
| :--- | :--- | :--- |
| Open Specific Product | `gather://product/:productId` | Product Detail Page (PDP) |
| Open Artisan Workshop | `gather://maker/:makerId` | Vendor Profile & Catalog |
| Filtered Category View | `gather://category/:categoryId?filter=verified` | Category Search with pre-applied chips |
| Resume Active Checkout | `gather://checkout/step/:stepNumber` | 3-Screen Checkout (Step 1, 2, or 3) |
| Merchant Dashboard Mode | `gather://vendor/overview` | Vendor Sales Analytics |
