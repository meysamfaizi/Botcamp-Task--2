# Account Menu UI

<p align="center">
  <a href="README.md">English</a> •
  <a href="README.fa.md"><bdi>فارسی</bdi></a>
</p>

![Preview](./asset/image/Preview%20.png)

- Live Demo: https://meysamfaizi.github.io/Botcamp-Task--2/
- Repository: https://github.com/meysamfaizi/Botcamp-Task--2

## Overview

A responsive right-to-left (RTL) user account menu card built with semantic HTML5 and modern CSS. The component includes a profile header with avatar and a list of navigation items, each paired with an inline SVG icon.

## The challenge

- Build a fully RTL layout that keeps icons, labels, and chevrons aligned correctly
- Use BEM naming for predictable, reusable class structure
- Keep icons crisp at any size using inline SVG instead of icon fonts
- Handle hover, focus, and active states accessibly
- Stay readable on small screens without breaking the card proportions

## Built with

- Semantic HTML5
- CSS Flexbox
- CSS custom properties (variables)
- BEM naming convention
- Inline SVG icons
- Media queries for responsive behavior
- Vazirmatn font (self-hosted via `@font-face`)
- `root` font-size at 62.5% for `rem`-based sizing

## Screenshots

| Desktop                                            | Mobile                                           |
| -------------------------------------------------- | ------------------------------------------------ |
| ![Desktop](./assets/images/screenshot-desktop.png) | ![Mobile](./assets/images/screenshot-mobile.png) |

## Project Structure

```text
Task2/
├── index.html
├── README.md
├── README.fa.md
├── Preview.jpg
├── assets/
│   ├── fonts/
│   └── images/
└── src/
├── font.css
└── style.css

## Features

- RTL-first layout with correct logical alignment
- Reusable `account-menu` block with BEM modifiers
- Accessible section labeling via `aria-label`
- Smooth transitions on interactive states
- Keyboard-focus visible styling
- Scalable inline SVG icons

## Getting Started

bash
git clone https://github.com/meysamfaizi/Botcamp-Task--2.git
cd Botcamp-Task--2

Then open `index.html` in a browser, or run it with the Live Server extension in VS Code.

## Continued Development

- Add keyboard navigation between menu items
- Introduce a dark theme using CSS variables
- Extract the menu into a reusable component
- Add subtle entrance animations

## Useful Resources

- [MDN — CSS Flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_flexible_box_layout)
- [MDN — Logical Properties](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_logical_properties_and_values)
- [BEM Methodology](https://getbem.com/)
- [Vazirmatn Font](https://github.com/rastikerdar/vazirmatn)

## Author

- Meysam Faizi
- GitHub: [@meysamfaizi](https://github.com/meysamfaizi)

## License

This project is licensed under the MIT License.

```
