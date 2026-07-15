# Bolt's Journal

## 2025-07-15 - Optimize Font Loading and Asset Delivery
**Learning:** Using `@import` inside inline CSS blocks blocks the renderer as the browser has to discover and load external font CSS sequentially rather than in parallel. Additionally, eagerly loading below-the-fold images increases initial page weight and network contention.
**Action:** Replace CSS `@import` with `<link rel="preconnect">` and `<link rel="stylesheet">` tags in the HTML `<head>`, and add `loading="lazy"` to off-screen images to improve FCP and LCP.
