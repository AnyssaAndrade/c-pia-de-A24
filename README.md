# A24 Website Clone (HTML & CSS Only)

## Overview

This project is a visual clone of the A24 website, built using only **HTML and CSS**. It was created as a hands-on exercise to better understand layout, positioning, and styling without relying on JavaScript or external frameworks.

The focus is on recreating the aesthetic and interaction patterns of the original site—especially the dynamic feel—using purely CSS techniques.

## Concept

The interface highlights a list of film titles. When hovering over each title, the background dynamically changes to a corresponding image or GIF, simulating interactivity without JavaScript.

This effect is achieved using CSS pseudo-elements and hover states.

## Features

* Minimalist header with navigation and branding
* Fullscreen background layout
* Hover-based background transitions using `::after`
* Typography styled with Google Fonts (**Anton**)
* Sticky header positioning
* Responsive scaling using viewport units

## Technologies Used

* HTML5
* CSS3

  * Flexbox
  * Positioning (absolute, fixed, sticky)
  * Pseudo-elements (`::after`)
  * Hover interactions

## Project Structure

```
/project-root
│
├── index.html
├── a24.css
└── /imagens
    ├── a24.png
    ├── search.png
    ├── weliveinatime.gif
    ├── heretic.gif
    ├── QUEER.webp
    ├── y2k.gif
    ├── TheBrutalist.webp
    └── babygirl.gif
```

## How It Works

Each film title (`.a1` to `.a6`) has a hover state that triggers a fullscreen background using a `::after` pseudo-element.

Example approach:

* The pseudo-element is positioned `fixed`
* It covers the entire viewport (`100vw` x `100vh`)
* A background image/GIF is applied
* `z-index: -1` keeps it behind the text

This creates the illusion of a dynamic background swap.

## Limitations

* No JavaScript → interactions are limited to hover states
* No support for touch-based hover (mobile experience is limited)
* Repetitive CSS structure (each title has its own class and rules)
* Fixed assets and hardcoded content

## What I Learned

* How to simulate interactivity using only CSS
* Managing layering with `z-index` and positioning
* Structuring layouts with Flexbox and absolute positioning
* Working with viewport-based sizing (`vw`, `vh`)
* Trade-offs of avoiding JavaScript in UI design

## Possible Improvements

* Refactor repeated CSS into reusable classes
* Add mobile-friendly interactions (e.g., click-based behavior with JS)
* Improve accessibility (semantic elements, alt text, keyboard navigation)
* Optimize image loading and performance
* Introduce transitions for smoother background changes

## Disclaimer

This project was created for educational purposes only.
All rights to the original design and content belong to A24.

---

*Built as a constraint-based experiment to push CSS as far as possible without JavaScript.*
