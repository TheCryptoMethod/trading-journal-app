```markdown
# Project Design System: Trader's Log & Analysis Web App

This document outlines the core design system for the Trader's Log & Analysis web application. The design emphasizes a modern, highly animated, and vibrant magenta-themed user interface, tailored for a SaaS product.

---

## 1. Color Palette

A vibrant and energetic color scheme built around a dominant magenta, complemented by electric blue and lime green, all set against a dark background.

*   **Primary:** `#FF33FF` (Electric Magenta) - Used for primary CTAs, key highlights, and dominant UI elements.
*   **Secondary:** `#33CCFF` (Electric Blue) - Used for secondary actions, complementary highlights, and gradients.
*   **Accent:** `#CCFF33` (Lime Green) - Used for success states, special callouts, and contrasting elements.
*   **Background:** `#1A1A1A` (Deep Charcoal) - The main background color, providing a dark canvas for vibrant elements.
*   **Surface:** `#2A2A2A` (Dark Gray) - Used for cards, panels, and component backgrounds.
*   **Text Primary:** `#F0F0F0` (Light Gray) - Main text color for readability on dark backgrounds.
*   **Text Secondary:** `#AAAAAA` (Medium Gray) - Used for secondary information, captions, and placeholders.
*   **Error:** `#FF4444` (Vivid Red) - For error messages and destructive actions.
*   **Warning:** `#FFBB00` (Amber Yellow) - For warning messages and alerts.
*   **Success:** `#00CC66` (Emerald Green) - For success messages and positive indicators.

---

## 2. Typography

A modern and highly readable sans-serif font pairing.

*   **Headings Font:** `Poppins` (Google Font)
    *   **H1:** `64px` (Desktop), `48px` (Tablet), `36px` (Mobile) - `font-weight: 700` (Bold), `line-height: 1.2`
    *   **H2:** `48px` (Desktop), `36px` (Tablet), `28px` (Mobile) - `font-weight: 600` (Semi-bold), `line-height: 1.2`
    *   **H3:** `32px` (Desktop), `28px` (Tablet), `24px` (Mobile) - `font-weight: 600` (Semi-bold), `line-height: 1.3`
    *   **H4:** `24px` (Desktop), `20px` (Tablet), `18px` (Mobile) - `font-weight: 500` (Medium), `line-height: 1.4`
*   **Body Font:** `Inter` (Google Font)
    *   **Body Large:** `18px` - `font-weight: 400` (Regular), `line-height: 1.6`
    *   **Body Regular:** `16px` - `font-weight: 400` (Regular), `line-height: 1.6`
    *   **Body Small:** `14px` - `font-weight: 400` (Regular), `line-height: 1.5`
    *   **Caption:** `12px` - `font-weight: 400` (Regular), `line-height: 1.5`
*   **Font Weights:** 400 (Regular), 500 (Medium), 600 (Semi-bold), 700 (Bold)

---

## 3. Spacing Scale

A consistent vertical and horizontal spacing scale based on multiples of 4px.

*   **xs:** `4px`
*   **sm:** `8px`
*   **md:** `16px`
*   **lg:** `32px`
*   **xl:** `64px`
*   **xxl:** `128px` (For large section padding)

---

## 4. Border Radius

Standardized border-radius values for UI elements.

*   **none:** `0px`
*   **sm:** `4px`
*   **md:** `8px`
*   **lg:** `16px`
*   **full:** `9999px` (For circular elements like avatars)

---

## 5. Shadow Styles

Subtle, modern shadows with a special magenta glow for interactive elements.

*   **none:** `none`
*   **sm:** `0px 2px 4px rgba(0, 0, 0, 0.2)`
*   **md:** `0px 4px 8px rgba(0, 0, 0, 0.3)`
*   **lg:** `0px 8px 16px rgba(0, 0, 0, 0.4)`
*   **magenta-glow:** `0px 0px 15px rgba(255, 51, 255, 0.7), 0px 0px 30px rgba(255, 51, 255, 0.3)` (Used for interactive element hovers/focus)

---

## 6. Component Specifications by Section

### General Component Principles:
*   All interactive elements (buttons, links, cards) will feature hover/focus states incorporating `color-primary` or `color-secondary` through subtle glows, color shifts, or background changes.
*   Gradients using `color-primary` and `color-secondary` will be strategically applied to enhance visual interest and dynamism.
*   Backgrounds will primarily be `color-background`, with components often using `color-surface` or a slightly darker variant to create depth.

---

### Hero Section

*   **Layout:** Full-width, vertically and horizontally centered content.
*   **Headline:** `H1` typography, `color-primary` or a gradient from `color-primary` to `color-secondary`.
*   **Subtext:** `Body Large` typography, `color-text-primary`.
*   **Call-to-Action (CTA) Button:**
    *   Large, prominent button.
    *   Background: `color-primary`.
    *   Text: `color-background`.
    *   Hover State: `color-primary` darkens slightly, `shadow-magenta-glow`.
*   **Animation Guidelines:**
    *   **Background:** A subtle, slow-moving particle effect or abstract geometric shapes (e.g., glowing lines, data points) in `color-primary` and `color-secondary` that gently shift and fade.
    *   **Headline:** Fade-in and subtle scale-up (`transform: scale(0.98)` to `scale(1)`) on page load.
    *   **CTA Button:** A subtle pulse effect on initial load, `shadow-magenta-glow` on hover.
    *   **Animated Elements:** Abstract trading charts or data visualizations subtly animating in the background, using `color-primary` and `color-secondary` to represent data flow or market movement.

---

### Features Section

*   **Layout:** Responsive grid of feature cards (3 columns desktop, 2 tablet, 1 mobile).
*   **Feature Card:**
    *   Background: `color-surface`, `border-radius-md`.
    *   Icon: Large, prominent icon using `color-primary` or `color-secondary`, often with a subtle glow.
    *   Title: `H3` typography, `color-text-primary`.
    *   Description: `Body Regular` typography, `color-text-primary`.
*   **Animation Guidelines:**
    *   **On Scroll:** Cards slide up (`transform: translateY(20px)`) and fade in (`opacity: 0` to `1`) with a staggered delay as they enter the viewport.
    *   **Hover:** Card lifts slightly (`transform: translateY(-5px)`), `shadow-md`, and a subtle border glow in `color-primary`. Icons within the card might have a subtle pulse or color shift.

---

### Pricing Section

*   **Layout:** Responsive grid of pricing cards (3 columns desktop, 2 tablet, 1 mobile). Includes a toggle for monthly/annual billing.
*   **Pricing Card:**
    *   Background: `color-surface` for standard tiers. A slightly darker magenta tint (e.g., `#3A1A3A`) for the "Most Popular" card. `border-radius-lg`.
    *   Title: `H3` typography, `color-text-primary`.
    *   Price: `H1` typography, `color-primary` or a gradient.
    *   Features List: `Body Regular` typography, `color-text-primary`, with checkmarks in `color-accent`.
    *   CTA Button:
        *   Background: `color-secondary`.
        *   Text: `color-background`.
        *   Hover State: `color-secondary` darkens, `shadow-magenta-glow`.
*   **Animation Guidelines:**
    *   **Toggle:** Smooth slide transition (`transform: translateX()`) for the toggle switch and a cross-fade (`opacity`) for price updates when switching between monthly/annual.
    *   **Card Hover:** Subtle scale-up (`transform: scale(1.02)`), `shadow-lg`, and a border glow in `color-primary`.
    *   **"Most Popular" Card:** May feature a continuous, very subtle breathing glow or pulsating border using `color-primary`.

---

### Testimonials Section

*   **Layout:** Carousel or grid of testimonial cards.
*   **Testimonial Card:**
    *   Background: `color-surface`, `border-radius-md`.
    *   Quote: `Body Large` typography, italic, `color-text-primary`.
    *   Avatar: Circular (`border-radius-full`), small border `2px solid color-primary`.
    *   Name: `Body Regular` typography, `color-text-primary`.
    *   Title/Company: `Body Small` typography, `color-text-secondary`.
*   **Animation Guidelines:**
    *   **Carousel:** Smooth slide transitions between testimonials.
    *   **Cards:** Subtle parallax effect on scroll, or slight scale-in (`transform: scale(0.98)` to `scale(1)`) on load.

---

### Contact Section

*   **Layout:** Two-column layout on desktop (form fields on one side, contact info/map on the other), stacked on mobile.
*   **Form Fields:**
    *   Background: `color-surface`, `border-radius-sm`, `border: 1px solid #444444`.
    *   Text: `color-text-primary`. Placeholder: `color-text-secondary`.
    *   Focus State: `border-color: color-primary`, subtle `shadow-magenta-glow`.
*   **Submit Button:**
    *   Background: `color-primary`.
    *   Text: `color-background`.
    *   Hover State: `color-primary` darkens, `shadow-magenta-glow`.
*   **Animation Guidelines:**
    *   **Form Fields:** Subtle slide-in (`transform: translateY(5px)`) or fade-in (`opacity`) on focus.
    *   **Submit Button:** A subtle pulse effect on hover.

---

### FAQ Section

*   **Layout:** Accordion style.
*   **Accordion Item:**
    *   Question: `H4` typography, `color-text-primary`, clickable area. Background `color-surface`, `border-radius-sm`.
    *   Answer: `Body Regular` typography, `color-text-primary`.
*   **Animation Guidelines:**
    *   **Expand/Collapse:** Smooth vertical slide transition (`max-height` or `height` animation) for the answer content. An icon (e.g., plus/minus) rotates (`transform: rotate()`) when expanded/collapsed.

---

### Footer Section

*   **Layout:** Multi-column on desktop (copyright, navigation links, social media icons), stacked on mobile.
*   **Links:** `Body Small` typography, `color-text-secondary`.
    *   Hover State: `color-primary`.
*   **Social Icons:** `color-text-secondary`.
    *   Hover State: `color-primary`, subtle scale-up (`transform: scale(1.1)`).
*   **Animation Guidelines:**
    *   **Links/Icons:** Subtle fade-in (`opacity`) and slight scale-up (`transform: scale()`) on hover.

---

## 7. Responsive Breakpoints

Standard breakpoints for consistent responsiveness across devices.

*   **Mobile:** `max-width: 767px`
*   **Tablet:** `min-width: 768px` and `max-width: 1023px`
*   **Desktop:** `min-width: 1024px`

---

## 8. Animation Guidelines

The UI is designed to be "highly animated" while maintaining a "subtle, professional" feel. This means animations are frequent and vibrant but always smooth, purposeful, and non-distracting.

*   **Overall Tone:** Energetic, dynamic, and engaging. Animations should enhance the user experience, not detract from it.
*   **Purpose:**
    *   **Visual Feedback:** Provide clear feedback for user interactions (hovers, clicks, form submissions).
    *   **Attention Guiding:** Direct user focus to key information or calls to action.
    *   **Brand Reinforcement:** Emphasize the modern, tech-savvy, and vibrant nature of the platform.
    *   **Engagement:** Add a sense of liveliness and sophistication to the interface.
*   **Key Properties for Animation:** `opacity`, `transform` (translate, scale, rotate), `color`, `background-color`, `box-shadow`. Avoid animating properties that cause layout reflows (e.g., `width`, `height` without `transform`) for performance.
*   **Easing:**
    *   **Interactive Elements:** `ease-out` or `cubic-bezier(0.25, 0.1, 0.25, 1)` for a quick, natural feel.
    *   **UI Transitions (e.g., accordion, carousel):** `ease-in-out` or `cubic-bezier(0.42, 0, 0.58, 1)` for a smoother, more controlled movement.
    *   **Background/Subtle Animations:** `linear` or very slow `ease-in-out` for continuous, non-intrusive motion.
*   **Duration:**
    *   **Fast (Hovers, small feedback):** `0.15s` - `0.2s`
    *   **Medium (Component reveals, UI transitions):** `0.3s` - `0.4s`
    *   **Slow (Background elements, subtle loops):** `2s` - `10s` (often looping indefinitely)
*   **Vibrancy vs. Professionalism:** The "highly animated" aspect comes from the *frequency* and *strategic use* of animations, often incorporating `color-primary` and `color-secondary` for visual flair. The "professional" aspect is maintained through smooth easing, appropriate durations, and ensuring animations are always purposeful and never jarring or excessive.
*   **Performance:** Prioritize CSS animations and hardware-accelerated transforms. Test animations across various devices, especially mobile, to ensure smooth performance.
*   **Accessibility:** Implement `prefers-reduced-motion` media query to provide a less animated experience for users with motion sensitivities. Animations should not be essential for understanding content or completing tasks.

---
```