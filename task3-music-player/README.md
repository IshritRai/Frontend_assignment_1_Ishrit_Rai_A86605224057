# Task 3 — Music Player & Playlist Shelf

A dark-mode mini music player with a spinning vinyl and an *Up Next* queue.
The two sections **stack on mobile** and sit **side-by-side from 768px**.

Open [`index.html`](index.html) in a browser and resize the window.

## How the requirements are met

| Requirement | Implementation (`style.css`) |
|-------------|------------------------------|
| Mobile stack, full-width rows | `.player { display:grid; grid-template-columns:1fr }`, `.track { width:100% }` |
| Desktop 200px + fluid grid | `@media (min-width: 768px) { .player { grid-template-columns: 200px 1fr } }` |
| Playlist rows | `.track { display:flex; justify-content:space-between; align-items:center }` |
| Playback controls | `.controls { display:flex; gap:0.75rem }` |
| Spinning vinyl | `@keyframes spin` → `animation: spin 6s linear infinite` |
| Row hover slide | `.track:hover { transform: translateX(6px) }` with `transition: transform 0.2s ease` |

Extras: vinyl drawn purely with CSS gradients, animated equaliser bars
(`scaleY` keyframes), progress fill via `scaleX`, accessible icon buttons and
`prefers-reduced-motion` support.
