## 2024-05-15 - Material Design Typography and Accessibility

**Learning:** When adopting Material Design typography, removing hardcoded font-sizes inline is not just about aesthetics but vastly improves accessibility. Using semantic tags like `<main>` and `<header>` combined with classes (e.g., `mat-display-3`, `mat-headline-4`) instead of `px` or `rem` values inline allows for better user scaling and screen-reader context.

**Action:** Standardize typographic components across all pages using defined CSS variables instead of inline styles, and map them to semantic HTML tags (`h1`, `h2`, `h3`, `p`) appropriately to ensure logical document hierarchy.

## 2024-05-15 - Premium UI Refactor

**Learning:** When moving from an outdated, purely visual CSS implementation to a modern, scalable design system (like Stripe or Apple), establishing a strict spacing grid (e.g., 8px increments) and a proportional typography scale is critical. Combining this with CSS variables allows for rapid, consistent styling across components and drastically reduces redundant CSS. Also, moving inline `<style>` blocks (like the overlay navigation) into the main stylesheet improves maintainability and separation of concerns.

**Action:** Always start a CSS refactor by defining root variables for colors, typography, spacing, and shadows before writing component styles. Avoid inline styles entirely.

## 2026-06-20 - DOM-based Menu Toggle Accessibility

**Learning:** When using custom DOM elements (like a `<span>`) as interactive toggles (e.g., an overlay menu), simply adding `role="button"` and `tabindex="0"` is insufficient. Screen readers require dynamic `aria-expanded` attributes to understand the current state of the menu (open vs. closed). This state must be manually managed via JavaScript alongside visual changes.

**Action:** Whenever implementing a custom interactive toggle component, ensure `aria-expanded` is applied and dynamically updated in the corresponding JavaScript open/close functions.
