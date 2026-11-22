# Responsive UI Mini-Components

Front-End Engineering Lab — **Practical Assignment: Responsive Web Design**

Four responsive web components built with semantic HTML and hand-written CSS
(no frameworks, no JavaScript), using Flexbox, CSS Grid, mobile-first media
queries, transitions and `@keyframes` animations.

| # | Component | Folder | Breakpoint |
|---|-----------|--------|------------|
| 1 | Product Showcase Card | [`task1-product-card`](task1-product-card/) | `min-width: 768px` |
| 2 | Responsive Pricing Cards | [`task2-pricing-cards`](task2-pricing-cards/) | `min-width: 850px` |
| 3 | Music Player & Playlist Shelf | [`task3-music-player`](task3-music-player/) | `min-width: 768px` |
| 4 | Creator Profile Header & Stats Card | [`task4-creator-profile`](task4-creator-profile/) | `min-width: 768px` |

## Running locally

No build step or dependencies are needed — open `index.html` (the landing page)
or any `taskN-*/index.html` file directly in a browser. To test responsiveness,
open DevTools → *Toggle device toolbar* and switch between a phone (< 768px)
and a desktop width.

## Project structure

```
.
├── index.html                  # landing page linking all tasks
├── task1-product-card/
│   ├── index.html
│   ├── style.css
│   ├── assets/desk-mat.svg
│   └── screenshots/
├── task2-pricing-cards/
│   ├── index.html
│   ├── style.css
│   └── screenshots/
├── task3-music-player/
│   ├── index.html
│   ├── style.css
│   └── screenshots/
└── task4-creator-profile/
    ├── index.html
    ├── style.css
    ├── assets/avatar.svg
    └── screenshots/
```

## Submission checklist

- [x] Viewport meta tag is included in `<head>` of every page
- [x] Universal `box-sizing: border-box` reset is applied
- [x] Mobile-first base layout stacks cleanly without horizontal scroll
- [x] Media queries activate multi-column layouts on wider screens
- [x] Flexbox handles 1D row/column alignment and button bars
- [x] CSS Grid handles 2D multi-column splits and equal stat grids
- [x] Hover transitions and `@keyframes` animations animate only `transform` / `opacity`
- [x] `prefers-reduced-motion` is respected

## Git workflow

Each task was developed on its own feature branch
(`feature/task1-product-card`, `feature/task2-pricing-cards`,
`feature/task3-music-player`, `feature/task4-creator-profile`) with small,
focused commits following the [Conventional Commits](https://www.conventionalcommits.org/)
style (`feat`, `style`, `fix`, `docs`, `a11y`, `chore`), then merged into
`main` with `--no-ff` merge commits so the history of every task is preserved.

## Author

**Ishrit Rai**
