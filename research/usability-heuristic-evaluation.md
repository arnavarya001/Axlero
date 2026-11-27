# Usability Heuristic Evaluation & UX Audit Matrix

> **Project:** gather. (Multi-Vendor Marketplace App)  
> **Evaluation Framework:** Nielsen Norman Group's 10 Usability Heuristics  
> **Audited Viewports:** iOS (`390 × 844 pt`) & Android (`360 × 800 dp`)  
> **Auditor:** Arnav Arya (Team Lead, Group 1)  
> **Date:** 27 November 2026

---

## 📊 Heuristic Evaluation Summary Matrix

| # | Heuristic Principle | Implementation in *gather.* | Compliance Status | Severity Rating (0–4) |
| :---: | :--- | :--- | :---: | :---: |
| **1** | **Visibility of System Status** | Sticky 3-step checkout bar (`Step 1/3 Address ➔ Step 2/3 Payment ➔ Step 3/3 Confirmed`), live stock warning pills (`Only 2 units left`), and cart count badge indicators. | ✅ Full Pass | 0 (None) |
| **2** | **Match Between System & Real World** | Artisanal terminology (`Handcrafted`, `Makers`, `Direct from Studio`), realistic item photos, and human-friendly shipping timeframes (`Arrives by Thursday, Nov 27`). | ✅ Full Pass | 0 (None) |
| **3** | **User Control & Freedom** | One-tap "Undo" snackbar when an item is removed from cart, clear back arrow `←` on all drill-down screens, and ability to edit shipping address in Step 2 without restarting checkout. | ✅ Full Pass | 0 (None) |
| **4** | **Consistency & Standards** | Strict adherence to iOS/Android design standards, uniform 8pt grid padding, persistent 5-tab bottom navigation, and unified Terracotta (`#A64028`) primary interactive states. | ✅ Full Pass | 0 (None) |
| **5** | **Error Prevention** | Phone number / PIN code format auto-masking, disabling the "Proceed to Pay" button until mandatory shipping fields are valid, and confirmation dialogs before deleting custom cart items. | ✅ Full Pass | 0 (None) |
| **6** | **Recognition Rather than Recall** | Persistent order summary drawer during payment step showing item thumbnails and vendor names, eliminating the need for buyers to memorize cart contents. | ✅ Full Pass | 0 (None) |
| **7** | **Flexibility & Efficiency of Use** | Fast-checkout accelerator: Saved UPI ID / Apple Pay one-tap biometric checkout, and horizontal quick-filter chips on category search screens. | ✅ Full Pass | 0 (None) |
| **8** | **Aesthetic & Minimalist Design** | Clean layout with generous whitespace, distraction-free checkout without third-party banner ads, and high contrast typography (WCAG 2.1 AA compliant). | ✅ Full Pass | 0 (None) |
| **9** | **Help Users Recognize & Recover from Errors** | Clear inline validation messages in red text (`#C2410C`) positioned directly below faulty form inputs, accompanied by clear corrective guidance (`Please enter a valid 6-digit PIN code`). | ✅ Full Pass | 0 (None) |
| **10** | **Help & Documentation** | Tooltip info pills explaining "Consolidated Shipping" and "Artisan Return Guarantees", plus direct "Chat with Maker" action on product detail pages. | ✅ Full Pass | 0 (None) |

---

## 🔍 Key Recommendations Implemented
1. **Consolidated Shipping Transparency:** Clear indication that multi-vendor items ship together without compounding delivery fees.
2. **Accessible Form Inputs:** Ensured all form labels remain visible as floating labels during text entry rather than disappearing placeholders.
