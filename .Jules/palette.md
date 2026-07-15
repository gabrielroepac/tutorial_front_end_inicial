# Palette's Journal - Tutorial: criando sua primeira página web

## 2025-07-15 - [Accessible Accordion & Navigation Controls]
**Learning:** For documentation-style pages with collapsing sections (accordions) and multi-step navigation, standard `div` tags with `onclick` actions are not accessible to keyboard or screen reader users. Changing them to proper semantic buttons/links and dynamically managing ARIA attributes (like `aria-expanded`, `aria-controls`, and `aria-current`) drastically improves screen reader feedback and accessibility.
**Action:** Always prefer standard HTML `<button>` or `<a>` elements for interactive elements, style their `:focus-visible` states explicitly, and keep stateful ARIA attributes synced with the JavaScript DOM changes.
