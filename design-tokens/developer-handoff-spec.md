# Developer Handoff & Redline Specifications

> **Workspace Reference:** `06-07 · Prototype & Handoff` ➔ `07_Developer Handoff · Specifications`  
> **Target Viewport:** Mobile iOS (`390 × 844 pt`) / Android (`360 × 800 dp`)  
> **Grid Architecture:** 8pt Rigid Spatial Grid (`4px`, `8px`, `16px`, `24px`, `32px`, `48px`)

---

## 📐 1. Global Layout Constraints & Margins

```
┌───────────────────────────────────────────────┐  0pt (Top Screen Edge)
│ [Status Bar] H: 44pt                          │
├───────────────────────────────────────────────┤  44pt
│ [Top Navigation Header] H: 64pt               │
│ - Screen Margins (Left / Right): 24pt         │
├───────────────────────────────────────────────┤  108pt
│                                               │
│ [Scrollable Content Body]                     │
│ - Content Container Width: 342pt              │
│ - Vertical Element Spacing: 16pt / 24pt       │
│                                               │
├───────────────────────────────────────────────┤  764pt
│ [Fixed Bottom Navigation Bar] H: 80pt         │
│ - Bottom Safe Area Inset: 16pt                │
└───────────────────────────────────────────────┘  844pt (Bottom Screen Edge)
```

---

## 🔲 2. Component Redlines & Padding Metrics

### A. Search Input Field
- **Dimensions:** Width `342px`, Height `48px`
- **Corner Radius:** `12px` (`radius-md`)
- **Border:** `1px solid #E5E0D8` (`color-border-subtle`)
- **Background:** `#FFFFFF` (`color-surface`)
- **Padding:** Left `16px`, Right `16px`, Vertical `12px`
- **Icon Size:** `20px × 20px`, Margin-right `12px`
- **Typography:** `14px / 20px`, Weight `400`, Color `#686E64`

### B. Standard Product Card (2-Column Grid)
- **Container Dimensions:** Width `162px`, Height `230px`
- **Image Area:** Width `162px`, Height `120px`, Radius Top `12px`
- **Content Padding:** `12px` on all sides
- **Spacing between title and price:** `4px`
- **Quick-Add CTA Button:**
  - Size: `30px × 30px`
  - Corner Radius: `6px`
  - Background: `#A64028` (`color-primary`)
  - Icon: `+` white `16px` bold

### C. Sticky Primary Action Button
- **Dimensions:** Height `48px`, Width `100%` (or fixed `186px` in dual-column bar)
- **Corner Radius:** `12px` (`radius-md`)
- **Background:** `#A64028` (`color-primary`)
- **Touch Target:** Minimum `48px × 48px` (Compliant with WCAG 2.1 AA Target Size)
- **Hover/Active State:** Background `#8C341F` (`color-primary-hover`)

---

## 🎨 3. CSS Implementation Snippets

### Elevation & Shadows
```css
/* Card Elevation Subtle */
.card-surface {
  background-color: #FFFFFF;
  border: 1px solid #E5E0D8;
  border-radius: 12px;
  box-shadow: 0 2px 4px rgba(34, 40, 32, 0.04), 0 1px 2px rgba(34, 40, 32, 0.02);
}

/* Floating Navigation Bar */
.bottom-nav-bar {
  position: fixed;
  bottom: 0;
  width: 100%;
  max-width: 390px;
  height: 80px;
  background-color: #FFFFFF;
  border-top: 1px solid #E5E0D8;
  padding: 8px 16px 20px 16px;
  display: flex;
  justify-content: space-around;
  align-items: center;
}
```

---

## 📱 4. Responsive Breakpoint Adaptation
- **Mobile Standard (`360px – 414px`):** Single column feed with 2-column product grid (`162px` card width).
- **Tablet / Large (`768px – 1024px`):** 4-column product grid, persistent left-rail navigation bar.
