```markdown
# Design System for Trading Journal Application

This document outlines the core design principles and specifications for the "Trading Journal" SaaS application. It aims to provide a consistent and professional user experience, leveraging a dark magenta aesthetic suitable for active daytraders.

---

## 1. Color Palette

The color palette is designed for a dark interface, prioritizing readability and a sophisticated feel, with magenta as the primary brand color.

| Variable Name           | Hex Code    | Description                                   |
| :---------------------- | :---------- | :-------------------------------------------- |
| `--color-primary`       | `#AD1457`   | Deep Magenta (Brand primary)                  |
| `--color-secondary`     | `#34495E`   | Dark Blue-Grey (Subtle contrast, secondary elements) |
| `--color-accent`        | `#E91E63`   | Vibrant Magenta (CTAs, highlights, active states) |
| `--color-background-main` | `#1A1A1A`   | Very Dark Grey (Main page background)         |
| `--color-background-card` | `#212121`   | Slightly Lighter Dark Grey (Card, elevated elements) |
| `--color-text-primary`  | `#E0E0E0`   | Light Grey (Main text, headings)              |
| `--color-text-secondary`| `#B0B0B0`   | Muted Grey (Secondary text, descriptions)     |
| `--color-success`       | `#4CAF50`   | Green (Positive feedback, profit)             |
| `--color-error`         | `#F44336`   | Red (Negative feedback, loss)                 |
| `--color-warning`       | `#FFC107`   | Amber (Warning, neutral alerts)               |

---

## 2. Typography

The `Inter` font family is chosen for its modern, clean, and highly readable characteristics across various weights and sizes.

*   **Font Family**: `Inter`, sans-serif
*   **Weights**: Regular (400), Medium (500), SemiBold (600), Bold (700)

| Element           | Font Size (px) | Font Weight | Line Height (em) | Color (Default)     |
| :---------------- | :------------- | :---------- | :--------------- | :------------------ |
| `--font-size-h1`  | 48px           | Bold (700)  | 1.2              | `--color-text-primary` |
| `--font-size-h2`  | 36px           | Bold (700)  | 1.2              | `--color-text-primary` |
| `--font-size-h3`  | 28px           | SemiBold (600)| 1.3              | `--color-text-primary` |
| `--font-size-h4`  | 24px           | SemiBold (600)| 1.3              | `--color-text-primary` |
| `--font-size-h5`  | 20px           | Medium (500)| 1.4              | `--color-text-primary` |
| `--font-size-h6`  | 18px           | Medium (500)| 1.4              | `--color-text-primary` |
| `--font-size-body`| 16px           | Regular (400)| 1.5              | `--color-text-primary` |
| `--font-size-small`| 14px           | Regular (400)| 1.5              | `--color-text-secondary` |
| `--font-size-button`| 18px           | SemiBold (600)| 1              | `--color-text-primary` |

---

## 3. Spacing Scale

A modular spacing scale based on an 8px grid system ensures consistent layout and visual hierarchy.

| Variable Name     | Pixel Value |
| :---------------- | :---------- |
| `--spacing-xs`    | 8px         |
| `--spacing-sm`    | 16px        |
| `--spacing-md`    | 24px        |
| `--spacing-lg`    | 40px        |
| `--spacing-xl`    | 64px        |
| `--spacing-xxl`   | 96px        |

---

## 4. Border Radius

Subtle border radii are used to soften edges and improve visual appeal without appearing overly rounded.

| Variable Name       | Pixel Value | Description                                |
| :------------------ | :---------- | :----------------------------------------- |
| `--border-radius-sm`| 4px         | Small elements (buttons, inputs)           |
| `--border-radius-md`| 8px         | Medium elements (cards, containers)        |
| `--border-radius-lg`| 12px        | Larger, prominent elements                 |

---

## 5. Shadow Styles

Shadows are used sparingly and subtly to provide depth and emphasize elevated elements on the dark background. The shadow color is a dark grey with varying opacity.

| Variable Name   | CSS Value                                 | Description                      |
| :-------------- | :---------------------------------------- | :------------------------------- |
| `--shadow-sm`   | `0 1px 3px rgba(0, 0, 0, 0.4)`            | Subtle lift (e.g., small buttons) |
| `--shadow-md`   | `0 4px 8px rgba(0, 0, 0, 0.5)`            | Standard elevation (e.g., cards) |
| `--shadow-lg`   | `0 10px 20px rgba(0, 0, 0, 0.6)`          | Prominent elevation (e.g., modals, hover states) |

---

## 6. Component Specifications by Section

### Hero Section

*   **Layout**: Full-width, centered content.
*   **Background**: `--color-background-main` with a subtle, abstract trading-related graphic or animation.
*   **Title**: `h1` (`--font-size-h1`), `Inter` Bold, `--color-text-primary`. Large, impactful, conveying the core value proposition.
*   **Subtitle**: `h3` (`--font-size-h3`), `Inter` Regular, `--color-text-secondary`. Explains the application's benefits concisely.
*   **Call to Action (CTA)**:
    *   **Button**: Primary button style.
    *   **Background**: `--color-accent`.
    *   **Text Color**: `--color-text-primary` (white).
    *   **Font**: `--font-size-button`, `Inter` SemiBold.
    *   **Border Radius**: `--border-radius-sm`.
    *   **Padding**: `16px` vertical, `32px` horizontal.
    *   **Hover**: Background darkens slightly, subtle scale up (`1.02`).
*   **Padding**: `--spacing-xl` vertical, `--spacing-lg` horizontal.

### Features Section

*   **Layout**: Grid of feature cards. Typically 2-3 columns on desktop, 1 column on mobile.
*   **Section Title**: `h2` (`--font-size-h2`), `Inter` Bold, `--color-text-primary`, centered.
*   **Feature Card**:
    *   **Background**: `--color-background-card`.
    *   **Border Radius**: `--border-radius-md`.
    *   **Shadow**: `--shadow-md`.
    *   **Icon**: Large (e.g., 48px), centered at top, `--color-accent`.
    *   **Title**: `h4` (`--font-size-h4`), `Inter` SemiBold, `--color-text-primary`.
    *   **Description**: Body text (`--font-size-body`), `Inter` Regular, `--color-text-secondary`.
    *   **Padding**: `--spacing-md`.
    *   **Hover**: Subtle lift (`--shadow-lg`, `transform: translateY(-4px)`).

### Pricing Section

*   **Layout**: Grid of pricing cards. Typically 3 columns on desktop, 1 column on mobile.
*   **Section Title**: `h2` (`--font-size-h2`), `Inter` Bold, `--color-text-primary`, centered.
*   **Pricing Card**:
    *   **Background**: `--color-background-card`.
    *   **Border Radius**: `--border-radius-md`.
    *   **Shadow**: `--shadow-md`.
    *   **Header**:
        *   **Plan Name**: `h3` (`--font-size-h3`), `Inter` SemiBold, `--color-text-primary`.
        *   **Price**: `h1` (`--font-size-h1`), `Inter` Bold, `--color-accent`.
        *   **Billing Cycle**: Body text (`--font-size-body`), `Inter` Regular, `--color-text-secondary`.
    *   **Features List**:
        *   Unordered list with checkmark icons (`--color-success`).
        *   Text: Body text (`--font-size-body`), `Inter` Regular, `--color-text-primary`.
    *   **Call to Action (CTA)**:
        *   **Button**: Primary button style.
        *   **Background**: `--color-accent`.
        *   **Text Color**: `--color-text-primary` (white).
        *   **Font**: `--font-size-button`, `Inter` SemiBold.
        *   **Border Radius**: `--border-radius-sm`.
        *   **Padding**: `14px` vertical, `28px` horizontal.
        *   **Hover**: Background darkens slightly, subtle scale up (`1.02`).
    *   **Highlight (e.g., "Pro" plan)**: May feature a `2px` border in `--color-primary` or a slightly darker background (`#2A2A2A`) to stand out.
    *   **Padding**: `--spacing-md` vertical, `--spacing-sm` horizontal.

### Footer Section

*   **Layout**: Dark background, typically multiple columns for navigation links, legal information, and social media.
*   **Background**: `--color-background-main` (or slightly darker, e.g., `#101010`).
*   **Links**:
    *   Text: Body text (`--font-size-body`), `Inter` Regular, `--color-text-secondary`.
    *   **Hover**: `--color-accent`, subtle underline.
*   **Copyright**: Small text (`--font-size-small`), `Inter` Regular, `--color-text-secondary`.
*   **Social Icons**:
    *   Color: `--color-text-secondary`.
    *   **Hover**: `--color-accent`.
*   **Padding**: `--spacing-lg` vertical, `--spacing-md` horizontal.

---

## 7. Responsive Breakpoints

The design is optimized for a mobile-first approach, adapting gracefully to larger screens.

*   **Mobile**: Up to `767px` (e.g., `max-width: 767px`)
*   **Tablet**: From `768px` to `1023px` (e.g., `min-width: 768px` and `max-width: 1023px`)
*   **Desktop**: From `1024px` and above (e.g., `min-width: 1024px`)

---

## 8. Animation Guidelines

Animations should be subtle, professional, and enhance the user experience without being distracting.

*   **Type**: Smooth transitions, subtle fades, and gentle transforms.
*   **Duration**: `200ms` to `300ms` for most interactive elements.
*   **Easing**: `ease-in-out` or `cubic-bezier(0.4, 0, 0.2, 1)` for a natural feel.
*   **Common Applications**:
    *   **Button Hovers**: Background color change, slight scale (`transform: scale(1.02)`).
    *   **Card Hovers**: Subtle lift (`transform: translateY(-4px)`) combined with a shadow change (`--shadow-lg`).
    *   **Link Hovers**: Color change, subtle underline or background highlight.
    *   **State Changes**: Gentle opacity or color transitions for active/inactive states.
*   **Principles**:
    *   **Purposeful**: Animations should serve a clear purpose (feedback, guidance, delight).
    *   **Performance**: Ensure animations run smoothly at 60fps on all target devices.
    *   **Subtle**: Avoid flashy or overly complex animations that could detract from the content.
```