# Design System for Trading Journal Application

This document outlines the core design system for the "Trading Journal" SaaS application, focusing on a dark theme and professional aesthetic.

---

## 1. Project Overview

*   **Project Name:** Trading Journal
*   **Type:** SaaS Web Application
*   **Style:** Dark Theme, Professional, Data-driven
*   **Goal:** Provide active day traders with advanced analytics and a robust backtesting engine.

---

## 2. Color Palette

A sophisticated dark theme with vibrant accents for data visualization and calls to action.

*   **Background Primary:** `#0A0A0A` (Deepest background, almost black)
*   **Background Secondary (Surface/Card):** `#1A1A1A` (Slightly lighter background for cards, panels)
*   **Background Tertiary (Hover/Active):** `#2C2C2C` (Subtle hover state for interactive elements)
*   **Primary Accent:** `#00C896` (Vibrant Teal Green - for positive metrics, primary CTAs, growth)
*   **Secondary Accent:** `#6A00FF` (Deep Violet - for secondary CTAs, distinct elements, alternative data highlights)
*   **Text Primary:** `#E0E0E0` (Light grey for main content text)
*   **Text Secondary:** `#A0A0A0` (Medium grey for secondary text, labels, descriptions)
*   **Text Disabled:** `#555555` (Darker grey for disabled states)
*   **Border/Divider:** `#333333` (Subtle dark grey for separators and borders)
*   **Success:** `#00E676` (Bright green for success messages, profit indicators)
*   **Error:** `#FF4D4D` (Red for error messages, loss indicators)
*   **Warning:** `#FFC107` (Amber for warning messages)
*   **Info:** `#00BFFF` (Light blue for informational messages)

---

## 3. Typography

Using `Inter` for both headings and body text ensures consistency, modern aesthetics, and excellent readability across all screen sizes.

*   **Font Family:** `Inter`, sans-serif
*   **Font Weights:** `400` (Regular), `500` (Medium), `600` (Semi-bold), `700` (Bold)

### Font Sizes (Base: 16px)

*   **H1:** `48px` (`font-weight: 700`, `line-height: 1.2`)
*   **H2:** `40px` (`font-weight: 700`, `line-height: 1.25`)
*   **H3:** `32px` (`font-weight: 600`, `line-height: 1.3`)
*   **H4:** `24px` (`font-weight: 600`, `line-height: 1.35`)
*   **H5:** `20px` (`font-weight: 500`, `line-height: 1.4`)
*   **H6:** `18px` (`font-weight: 500`, `line-height: 1.45`)
*   **Body Large:** `18px` (`font-weight: 400`, `line-height: 1.6`)
*   **Body:** `16px` (`font-weight: 400`, `line-height: 1.6`)
*   **Small:** `14px` (`font-weight: 400`, `line-height: 1.5`)
*   **Extra Small:** `12px` (`font-weight: 400`, `line-height: 1.4`)

---

## 4. Spacing Scale

A modular spacing scale based on a 4px grid, ensuring consistent vertical and horizontal rhythm.

*   **xs:** `4px`
*   **sm:** `8px`
*   **md:** `16px`
*   **lg:** `24px`
*   **xl:** `32px`
*   **xxl:** `48px`
*   **xxxl:** `64px`

---

## 5. Border Radius

Subtle rounding for a modern, approachable feel without being overly soft.

*   **sm:** `4px` (For small elements like buttons, input fields)
*   **md:** `8px` (For cards, containers)
*   **lg:** `12px` (For larger components, modals)
*   **full:** `9999px` (For pills, avatars)

---

## 6. Shadow Styles

Subtle, diffused shadows suitable for a dark theme to provide depth without harshness.

*   **shadow-sm:** `0 2px 4px rgba(0, 0, 0, 0.3)` (For subtle lift on interactive elements)
*   **shadow-md:** `0 4px 12px rgba(0, 0, 0, 0.4)` (For cards, panels)
*   **shadow-lg:** `0 8px 24px rgba(0, 0, 0, 0.6)` (For modals, dropdowns, elevated components)
*   **shadow-inset:** `inset 0 1px 3px rgba(0, 0, 0, 0.5)` (For pressed states or subtle inner depth)

---

## 7. Component Specifications by Section

### 7.1. Hero Section

*   **Layout:** Full-width, content centered horizontally and vertically.
*   **Headline (H1):** `color-text-primary`, `font-weight: 700`. Emphasizes the core value proposition.
*   **Sub-headline (Body Large):** `color-text-secondary`. Provides supporting details.
*   **Primary CTA Button:** `background-color: color-primary-accent`, `color: #0A0A0A`, `border-radius: border-radius-sm`, `padding: spacing-md spacing-lg`.
*   **Secondary CTA Button (Optional):** `background-color: transparent`, `color: color-text-primary`, `border: 1px solid color-border-divider`, `border-radius: border-radius-sm`, `padding: spacing-md spacing-lg`.
*   **Visual Element:** Large, high-quality screenshot or video loop of the application interface, subtly animated, positioned to the side or below the text.

### 7.2. Features Section

*   **Layout:** Grid of feature cards (2-4 columns on desktop, 1-2 columns on tablet, 1 column on mobile).
*   **Section Title (H2):** `color-text-primary`, centered.
*   **Feature Card:**
    *   `background-color: color-background-secondary`, `border-radius: border-radius-md`, `padding: spacing-xl`, `shadow: shadow-md`.
    *   **Icon:** Large, prominent icon (e.g., SVG), `color: color-primary-accent`.
    *   **Title (H3):** `color-text-primary`, `margin-top: spacing-md`.
    *   **Description (Body):** `color-text-secondary`, `margin-top: spacing-sm`.

### 7.3. Pricing Section

*   **Layout:** Grid of pricing cards (3 columns on desktop, 1-2 columns on tablet, 1 column on mobile).
*   **Section Title (H2):** `color-text-primary`, centered.
*   **Billing Toggle:** Segmented control for "Monthly" / "Annually" with `background-color: color-background-secondary`, `color-text-secondary` for inactive, `color-primary-accent` for active.
*   **Pricing Card:**
    *   `background-color: color-background-secondary`, `border-radius: border-radius-md`, `padding: spacing-xl`, `shadow: shadow-md`.
    *   **Plan Name (H3):** `color-text-primary`, centered.
    *   **Price (H2):** `color-primary-accent`, `font-weight: 700`, centered. Includes currency symbol and billing cycle (e.g., "/month").
    *   **Features List (UL):** `color-text-primary`, `list-style: none`, `padding: 0`, `margin-top: spacing-lg`. Each list item includes a checkmark icon (`color-success`).
    *   **CTA Button:** `background-color: color-primary-accent` (or `color-secondary-accent` for premium plans), `color: #0A0A0A`, `border-radius: border-radius-sm`, `padding: spacing-md spacing-lg`, `margin-top: spacing-xl`.

### 7.4. Testimonials Section

*   **Layout:** Carousel or grid of testimonial cards (1-2 columns on desktop, 1 column on tablet/mobile).
*   **Section Title (H2):** `color-text-primary`, centered.
*   **Testimonial Card:**
    *   `background-color: color-background-secondary`, `border-radius: border-radius-md`, `padding: spacing-xl`, `shadow: shadow-md`.
    *   **Quote (Body Large):** `color-text-primary`, `font-style: italic`, `margin-bottom: spacing-md`.
    *   **Author Avatar:** Circular image, `width: 48px`, `height: 48px`, `border-radius: border-radius-full`.
    *   **Author Name (H5):** `color-text-primary`, `margin-left: spacing-sm`.
    *   **Author Title (Small):** `color-text-secondary`, `margin-left: spacing-sm`.

### 7.5. FAQ Section

*   **Layout:** Accordion component.
*   **Section Title (H2):** `color-text-primary`, centered.
*   **Accordion Item:**
    *   **Question (H4):** `color-text-primary`, `padding: spacing-md`, `background-color: color-background-secondary`, `border-radius: border-radius-sm`. Includes an expand/collapse icon (e.g., chevron).
    *   **Answer (Body):** `color-text-secondary`, `padding: spacing-md`, `background-color: color-background-secondary`, `border-radius: border-radius-sm`, `margin-top: spacing-xs` (only visible when expanded).

### 7.6. Footer Section

*   **Layout:** Multi-column grid on desktop, stacked on mobile.
*   **Background:** `color-background-primary`, `padding: spacing-xxl 0`.
*   **Logo:** Project logo.
*   **Navigation Links:** Grouped by category (e.g., Product, Company, Resources). Each link is `color-text-secondary` with `color-text-primary` on hover.
*   **Social Media Icons:** Icons for platforms like Twitter, LinkedIn, etc., `color-text-secondary` with `color-primary-accent` on hover.
*   **Copyright:** `color-text-secondary`, `font-size: font-size-small`.

---

## 8. Responsive Breakpoints

Standard breakpoints for optimal viewing across devices.

*   **Mobile:** `0px - 767px`
*   **Tablet:** `768px - 1023px`
*   **Desktop:** `1024px - 1439px`
*   **Large Desktop:** `1440px+`

---

## 9. Animation Guidelines

Animations should be subtle, professional, and enhance user experience without being distracting.

*   **Duration:**
    *   `fast`: `150ms` (e.g., button hovers, small state changes)
    *   `normal`: `250ms` (e.g., card hovers, modal transitions)
    *   `slow`: `400ms` (e.g., complex component transitions, page transitions)
*   **Timing Function:**
    *   `ease-in-out`: For most UI interactions (smooth start and end).
    *   `ease-out`: For elements appearing (quick start, gentle end).
    *   `linear`: For continuous animations (e.g., loading spinners).
*   **Properties:** Focus on `opacity`, `transform` (translate, scale), `background-color`, `border-color`, `box-shadow`.
*   **Examples:**
    *   **Button Hover:** `background-color` and `transform: translateY(-2px)` with `ease-in-out` `150ms`.
    *   **Card Hover:** `box-shadow` and `transform: translateY(-4px)` with `ease-in-out` `250ms`.
    *   **Modal Entry/Exit:** `opacity` and `transform: translateY(20px)` with `ease-out` `250ms`.
    *   **Accordion Toggle:** `height` and `opacity` with `ease-in-out` `250ms`.