## 2024-05-15 - Material Design Typography and Accessibility

**Learning:** When adopting Material Design typography, removing hardcoded font-sizes inline is not just about aesthetics but vastly improves accessibility. Using semantic tags like `<main>` and `<header>` combined with classes (e.g., `mat-display-3`, `mat-headline-4`) instead of `px` or `rem` values inline allows for better user scaling and screen-reader context.

**Action:** Standardize typographic components across all pages using defined CSS variables instead of inline styles, and map them to semantic HTML tags (`h1`, `h2`, `h3`, `p`) appropriately to ensure logical document hierarchy.
