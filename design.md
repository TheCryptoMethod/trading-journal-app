# Design System for Trading Journal Application

This document outlines the core design principles and specifications for the "Trading Journal" SaaS application. The goal is to create a professional, data-focused, and visually engaging experience for active daytraders, leveraging a dark aesthetic with a distinct magenta accent.

---

## 1. Color Palette

A dark, sophisticated palette with a vibrant magenta primary color and a contrasting accent for key interactions and data visualization.

*   **Primary (Brand Magenta):** `#A30062`
    *   *Usage:* Main branding, primary CTAs, active states, key data highlights.
*   **Secondary (Deep Blue):** `#0062A3`
    *   *Usage:* Complementary elements, secondary buttons, background for specific sections, charts.
*   **Accent (Electric Cyan):** `#00FFFF`
    *   *Usage:* Interactive elements, alerts, data points requiring high visibility, profit indicators.
*   **Background (Dark Grey):** `#121212`
    *   *Usage:* Main application background, card backgrounds, panels.
*   **Surface (Slightly Lighter Dark Grey):** `#1E1E1E`
    *   *Usage:* Card backgrounds, modal backgrounds, input fields.
*   **Text (Light Grey):** `#E0E0E0`
    *   *Usage:* Primary body text, labels.
*   **Text Secondary (Muted Grey):** `#A0A0A0`
    *   *Usage:* Secondary information, helper text, disabled states.
*   **Success:** `#00C853`
    *   *Usage:* Positive feedback, profit indicators.
*   **Error:** `#D32F2F`
    *   *Usage:* Negative feedback, loss indicators, error messages.
*   **Warning:** `#FFC107`
    *   *Usage:* Cautionary messages, neutral alerts.

---

## 2. Typography

A clean, modern sans-serif font for optimal readability across all content.

*   **Headings Font:** `Inter` (or a suitable web-safe fallback like `sans-serif`)
*   **Body Font:** `Inter` (or a suitable web-safe fallback like `sans-serif`)

### Font Sizes

*   **H1:** `48px` (Line-height: `1.2`)
*   **H2:** `36px` (Line-height: `1.25`)
*   **H3:** `28px` (Line-height: `1.3`)
*   **H4:** `24px` (Line-height: `1.35`)
*   **H5:** `20px` (Line-height: `1.4`)
*   **H6:** `18px` (Line-height: `1.45`)
*   **Body Large:** `18px` (Line-height: `1.5`)
*   **Body:** `16px` (Line-height: `1.5`)
*   **Small:** `14px` (Line-height: `1.6`)
*   **Extra Small:** `12px` (Line-height: `1.6`)

### Font Weights

*   **Regular:** `400`
*   **Medium:** `500`
*   **Semi-Bold:** `600`
*   **Bold:** `700`

---

## 3. Spacing Scale

A consistent 8px grid-based spacing system for all elements.

*   **xs:** `4px`
*   **sm:** `8px`
*   **md:** `16px`
*   **lg:** `32px`
*   **xl:** `64px`
*   **xxl:** `128px`

---

## 4. Border Radius

Subtle border radius for a modern, soft aesthetic.

*   **Default:** `4px`
*   **Pill (for tags/badges):** `9999px` (fully rounded)

---

## 5. Shadow Styles

Subtle, dark shadows to provide depth without overpowering the dark background.

*   **shadow-sm:** `0px 1px 3px rgba(0, 0, 0, 0.4)`
*   **shadow-md:** `0px 4px 6px rgba(0, 0, 0, 0.6)`
*   **shadow-lg:** `0px 10px 15px rgba(0, 0, 0, 0.8)`
*   **shadow-inset (for subtle inner depth):** `inset 0px 1px 3px rgba(0, 0, 0, 0.6)`

---

## 6. Component Specifications

### 6.1. Hero Section

*   **Background:** `background-color: #121212;` (main dark background)
*   **Headline (H1):** `font-size: 48px; font-weight: 700; color: #E0E0E0;`
    *   *Content:* "Master Your Trades. Maximize Your Profits."
*   **Subheadline (Body Large):** `font-size: 18px; font-weight: 400; color: #A0A0A0;`
    *   *Content:* "Advanced analytics and backtesting for active daytraders."
*   **Primary CTA Button:**
    *   `background-color: #A30062;`
    *   `color: #E0E0E0;`
    *   `padding: 16px 32px;`
    *   `border-radius: 4px;`
    *   `font-size: 18px; font-weight: 600;`
    *   `box-shadow: 0px 4px 6px rgba(163, 0, 98, 0.4);`
    *   *Hover:* `background-color: #C20075;`
    *   *Content:* "Start Free Trial"
*   **Secondary CTA Button (Optional):**
    *   `background-color: transparent;`
    *   `border: 1px solid #A30062;`
    *   `color: #A30062;`
    *   `padding: 16px 32px;`
    *   `border-radius: 4px;`
    *   `font-size: 18px; font-weight: 600;`
    *   *Hover:* `background-color: rgba(163, 0, 98, 0.1);`
    *   *Content:* "Learn More"
*   **Imagery/Illustration:** Abstract data visualization, trading charts, or a stylized device mockup displaying the app UI. Predominantly dark tones with magenta and cyan highlights.

### 6.2. Features Section

*   **Section Title (H2):** `font-size: 36px; font-weight: 700; color: #E0E0E0;`
    *   *Content:* "Unlock Your Trading Potential"
*   **Feature Card:**
    *   `background-color: #1E1E1E;`
    *   `padding: 32px;`
    *   `border-radius: 4px;`
    *   `box-shadow: 0px 1px 3px rgba(0, 0, 0, 0.4);`
    *   **Icon:** `font-size: 48px; color: #00FFFF;` (or gradient with #A30062)
    *   **Feature Title (H4):** `font-size: 24px; font-weight: 600; color: #E0E0E0;`
    *   **Feature Description (Body):** `font-size: 16px; font-weight: 400; color: #A0A0A0;`
*   **Layout:** Responsive grid (e.g., 3 columns on desktop, 2 on tablet, 1 on mobile).

### 6.3. Pricing Section

*   **Section Title (H2):** `font-size: 36px; font-weight: 700; color: #E0E0E0;`
    *   *Content:* "Simple, Transparent Pricing"
*   **Pricing Card:**
    *   `background-color: #1E1E1E;`
    *   `padding: 32px;`
    *   `border-radius: 4px;`
    *   `box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.6);`
    *   **Plan Name (H3):** `font-size: 28px; font-weight: 700; color: #E0E0E0;`
    *   **Price (H1):** `font-size: 48px; font-weight: 700; color: #A30062;` (e.g., "$49")
    *   **Price Suffix (Body Small):** `font-size: 14px; color: #A0A0A0;` (e.g., "/month")
    *   **Feature List Item (Body):** `font-size: 16px; color: #E0E0E0;` with checkmark icon (`color: #00C853;`)
    *   **CTA Button:**
        *   `background-color: #A30062;`
        *   `color: #E0E0E0;`
        *   `padding: 12px 24px;`
        *   `border-radius: 4px;`
        *   `font-size: 16px; font-weight: 600;`
        *   *Hover:* `background-color: #C20075;`
        *   *Content:* "Choose Plan"
*   **Highlighted Plan (e.g., "Most Popular"):**
    *   `border: 2px solid #A30062;`
    *   `background-color: #2A001A;` (slightly darker magenta-tinted background)
    *   Optional "Popular" badge: `background-color: #00FFFF; color: #121212; padding: 4px 8px; border-radius: 4px; font-size: 12px; font-weight: 700;`

### 6.4. Footer Section

*   **Background:** `background-color: #0A0A0A;` (slightly darker than main background)
*   **Text (Body Small):** `font-size: 14px; color: #A0A0A0;`
*   **Links:** `color: #A0A0A0;`
    *   *Hover:* `color: #A30062; text-decoration: underline;`
*   **Copyright:** `font-size: 14px; color: #A0A0A0;`
    *   *Content:* "© [Year] Trading Journal. All rights reserved."
*   **Social Media Icons:** `color: #A0A0A0; font-size: 24px;`
    *   *Hover:* `color: #A30062;`
*   **Layout:** Typically 3-4 columns for links on desktop, stacked on mobile.

---

## 7. Responsive Breakpoints

Standard breakpoints for adapting the layout across devices.

*   **Mobile:** `0px - 767px`
*   **Tablet:** `768px - 1023px`
*   **Desktop:** `1024px +`

---

## 8. Animation Guidelines

Animations should be subtle, professional, and enhance the user experience without being distracting.

*   **Duration:** `200ms - 300ms` for most interactive elements (buttons, links, card hovers).
*   **Easing:** `ease-in-out` for smooth transitions.
*   **Properties:**
    *   **Opacity:** For fades, showing/hiding elements.
    *   **Transform:** For subtle scaling (`scale(1.02)`), translations (`translateY(-2px)`), or rotations (e.g., for icons).
    *   **Background-color:** For button hovers, active states.
    *   **Border-color:** For input focus states.
*   **Examples:**
    *   Button hover: `background-color` change, slight `transform: translateY(-2px);`
    *   Card hover: `box-shadow` increase, slight `transform: translateY(-4px);`
    *   Menu open/close: `opacity` and `transform` (e.g., slide in from top/side).
    *   Data updates: Subtle `opacity` or `background-color` flash for new data points.