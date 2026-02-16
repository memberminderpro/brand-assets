# Brand Assets

This repository, `brand-assets`, is a collection of assets for use in projects that need to adhere to **Member Minder Pro, LLC** branding. It includes CSS files containing brand color variables (MemberMinder Pro and, for convenience, Rotary International), typography references, and image assets such as logos and icons for Member Minder Pro and its related family of products and brands.

Use these assets and definitions as the **single source of truth** when implementing or extending Member Minder Pro branding across applications, themes, documentation, and marketing materials.

---

## About Member Minder Pro brand elements

This repository is the authoritative source for Member Minder Pro brand colors and typography. When using these assets:

- **Colors** — Use the CSS variables in `css/colors.css` so that hex, RGB, and HSL stay consistent across projects.
- **Logos and graphics** — Use the provided logos and icons from `img/`; avoid altering proportions or colors outside the defined palette.
- **Typography** — Follow any typography definitions referenced in this repo (e.g. in CSS or documentation) for a consistent voice across products.

---

## Contents of this repository

1. **CSS (brand colors and tokens)**
   - `css/colors.css`: CSS custom properties for Member Minder Pro’s full color systems (MMP Blue, Red, UI Blue, Gold, Green, Off-White, Gray) plus Rotary International colors. Each family includes main, light, dark, and hover shades. Use these variables in web and app projects for consistent brand colors.

2. **Image assets**
   - **Logos** — `img/logos/`: Member Minder Pro logos (e.g. `mmp-logo-color.svg`, `mmp-logo-white.svg`, `MMP-LOGO-REDWHITE.svg`, `mmp-simple-logo-color.svg`).
   - **Icons** — `img/icons/`: MMP app icons and mark (e.g. `mmp-icon.svg`, `memberminderpro.svg`), text-only lockups, and social/third-party badges (e.g. App Store, social brands) as provided.
   - **Theme / messaging** — `img/theme-message/`: Supporting artwork (e.g. `unite-for-good.svg`) for use in approved contexts.

---

## Usage

### CSS brand colors

Include `css/colors.css` in your project, then use the variables in your own CSS.

#### Local or build pipeline

```html
<link rel="stylesheet" href="path/to/css/colors.css">
```

#### CDN (GitHub)

You can load the root color library directly from this repository so you don’t have to host or bundle the file yourself.

**Raw GitHub file** — Use the raw file URL (replace `owner`, `repo`, and `branch` with the actual repository and branch, e.g. `main`):

```html
<link rel="stylesheet" href="https://raw.githubusercontent.com/owner/repo/branch/css/colors.css">
```

**jsDelivr (recommended)** — [jsDelivr](https://www.jsdelivr.com/) serves GitHub files with caching and better availability. Use this form (replace `owner`, `repo`, and `branch` as above):

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/owner/repo@branch/css/colors.css">
```

Example for the canonical repo on the `main` branch:

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/memberminderpro/brand-assets@main/css/colors.css">
```

Pin to a specific release by using a tag instead of a branch (e.g. `@v1.0.0`), when available.

In your CSS:

```css
:root {
  /* Already provided by colors.css; override only if needed */
}

.header {
  background-color: var(--mmp-blue);
  color: var(--mmp-offwhite);
}

.cta {
  background-color: var(--mmp-ui-blue);
  color: var(--mmp-blue-dark);
}
```

For the full set of shades (e.g. `--mmp-blue-light`, `--mmp-ui-blue-hover`), see `css/colors.css`.

### Logos and icons

Use the SVG or PNG assets from `img/logos/` and `img/icons/` directly in HTML or in your build pipeline. Prefer SVG for resolution independence.

```html
<img src="path/to/img/logos/mmp-logo-color.svg" alt="Member Minder Pro">
<img src="path/to/img/icons/mmp-icon.svg" alt="Member Minder Pro icon">
```

Resize via CSS or `width`/`height`; do not stretch or distort. Use the correct light/dark or color/white variant for your background (e.g. dark background → white logo).

---

## MemberMinder Pro Brand Assets: Color Palette

This document provides the visual swatches and technical definitions for the MemberMinder Pro color system. All colors are defined as CSS variables in [colors.css](https://github.com/memberminderpro/brand-assets/blob/main/css/colors.css).

---

### MemberMinder Pro Primary Palette
The main identity colors used for branding, logos, and primary UI elements.

| Swatch | Color Name | CSS Variable | Hex Code | RGB | HSL |
| :---: | :--- | :--- | :--- | :--- | :--- |
| ![](https://singlecolorimage.com/get/1e224e/20x20) | MMP Blue | `--mmp-blue` | `#1e224e` | `rgb(30, 34, 78)` | `hsl(235, 44%, 21%)` |
| ![](https://singlecolorimage.com/get/841c30/20x20) | MMP Red | `--mmp-red` | `#841c30` | `rgb(132, 28, 48)` | `hsl(348, 65%, 31%)` |
| ![](https://singlecolorimage.com/get/8dafd3/20x20) | MMP UI Blue | `--mmp-ui-blue` | `#8dafd3` | `rgb(141, 175, 211)` | `hsl(211, 44%, 69%)` |
| ![](https://singlecolorimage.com/get/c9a967/20x20) | MMP Gold | `--mmp-gold` | `#c9a967` | `rgb(201, 169, 103)` | `hsl(40, 49%, 60%)` |
| ![](https://singlecolorimage.com/get/7a9d8e/20x20) | MMP UI Green | `--mmp-ui-green` | `#7a9d8e` | `rgb(122, 157, 142)` | `hsl(154, 15%, 55%)` |
| ![](https://singlecolorimage.com/get/f8f8f8/20x20) | MMP Off-White | `--mmp-offwhite` | `#f8f8f8` | `rgb(248, 248, 248)` | `hsl(0, 0%, 97%)` |
| ![](https://singlecolorimage.com/get/9f9ea5/20x20) | MMP Gray | `--mmp-gray` | `#9f9ea5` | `rgb(159, 158, 165)` | `hsl(249, 4%, 63%)` |

---

## MMP Blue Shade System
| Swatch | Weight | CSS Variable | Hex Code | RGB | HSL |
| :---: | :--- | :--- | :--- | :--- | :--- |
| ![](https://singlecolorimage.com/get/eff0f7/20x20) | Ultra Light | `--mmp-blue-ultra-light` | `#eff0f7` | `rgb(239, 240, 247)` | `hsl(232, 33%, 95%)` |
| ![](https://singlecolorimage.com/get/cfd2e6/20x20) | Light | `--mmp-blue-light` | `#cfd2e6` | `rgb(207, 210, 230)` | `hsl(232, 33%, 86%)` |
| ![](https://singlecolorimage.com/get/6a72b0/20x20) | Semi Light | `--mmp-blue-semi-light` | `#6a72b0` | `rgb(106, 114, 176)` | `hsl(233, 31%, 55%)` |
| ![](https://singlecolorimage.com/get/1e224e/20x20) | **Main** | `--mmp-blue` | `#1e224e` | `rgb(30, 34, 78)` | `hsl(235, 44%, 21%)` |
| ![](https://singlecolorimage.com/get/171a39/20x20) | Hover | `--mmp-blue-hover` | `#171a39` | `rgb(23, 26, 57)` | `hsl(235, 43%, 16%)` |
| ![](https://singlecolorimage.com/get/151737/20x20) | Semi Dark | `--mmp-blue-semi-dark` | `#151737` | `rgb(21, 23, 55)` | `hsl(236, 45%, 15%)` |
| ![](https://singlecolorimage.com/get/0e1025/20x20) | Dark | `--mmp-blue-dark` | `#0e1025` | `rgb(14, 16, 37)` | `hsl(235, 45%, 10%)` |
| ![](https://singlecolorimage.com/get/070812/20x20) | Ultra Dark | `--mmp-blue-ultra-dark` | `#070812` | `rgb(7, 8, 18)` | `hsl(235, 44%, 5%)` |

## MMP Red Shade System
| Swatch | Weight | CSS Variable | Hex Code | RGB | HSL |
| :---: | :--- | :--- | :--- | :--- | :--- |
| ![](https://singlecolorimage.com/get/fce9ed/20x20) | Ultra Light | `--mmp-red-ultra-light` | `#fce9ed` | `rgb(252, 233, 237)` | `hsl(347, 73%, 95%)` |
| ![](https://singlecolorimage.com/get/f3bcc9/20x20) | Light | `--mmp-red-light` | `#f3bcc9` | `rgb(243, 188, 201)` | `hsl(346, 70%, 85%)` |
| ![](https://singlecolorimage.com/get/db4d6b/20x20) | Semi Light | `--mmp-red-semi-light` | `#db4d6b` | `rgb(219, 77, 107)` | `hsl(347, 67%, 58%)` |
| ![](https://singlecolorimage.com/get/841c30/20x20) | **Main** | `--mmp-red` | `#841c30` | `rgb(132, 28, 48)` | `hsl(348, 65%, 31%)` |
| ![](https://singlecolorimage.com/get/6f1728/20x20) | Hover | `--mmp-red-hover` | `#6f1728` | `rgb(111, 23, 40)` | `hsl(348, 66%, 26%)` |
| ![](https://singlecolorimage.com/get/5d1423/20x20) | Semi Dark | `--mmp-red-semi-dark` | `#5d1423` | `rgb(93, 20, 35)` | `hsl(348, 65%, 22%)` |
| ![](https://singlecolorimage.com/get/3f0e18/20x20) | Dark | `--mmp-red-dark` | `#3f0e18` | `rgb(63, 14, 24)` | `hsl(348, 64%, 15%)` |
| ![](https://singlecolorimage.com/get/22070c/20x20) | Ultra Dark | `--mmp-red-ultra-dark` | `#22070c` | `rgb(34, 7, 12)` | `hsl(349, 66%, 8%)` |

## MMP UI Blue Shade System
| Swatch | Weight | CSS Variable | Hex Code | RGB | HSL |
| :---: | :--- | :--- | :--- | :--- | :--- |
| ![](https://singlecolorimage.com/get/e1f0ff/20x20) | Ultra Light | `--mmp-ui-blue-ultra-light` | `#e1f0ff` | `rgb(225, 240, 255)` | `hsl(210, 100%, 94%)` |
| ![](https://singlecolorimage.com/get/afd2f7/20x20) | Light | `--mmp-ui-blue-light` | `#afd2f7` | `rgb(175, 210, 247)` | `hsl(211, 84%, 83%)` |
| ![](https://singlecolorimage.com/get/7293b5/20x20) | Semi Light | `--mmp-ui-blue-semi-light` | `#7293b5` | `rgb(114, 147, 181)` | `hsl(210, 31%, 58%)` |
| ![](https://singlecolorimage.com/get/8dafd3/20x20) | **Main** | `--mmp-ui-blue` | `#8dafd3` | `rgb(141, 175, 211)` | `hsl(211, 44%, 69%)` |
| ![](https://singlecolorimage.com/get/b0d3f8/20x20) | Hover | `--mmp-ui-blue-hover` | `#b0d3f8` | `rgb(176, 211, 248)` | `hsl(211, 84%, 83%)` |
| ![](https://singlecolorimage.com/get/1e3c5b/20x20) | Semi Dark | `--mmp-ui-blue-semi-dark` | `#1e3c5b` | `rgb(30, 60, 91)` | `hsl(211, 50%, 24%)` |
| ![](https://singlecolorimage.com/get/04233f/20x20) | Dark | `--mmp-ui-blue-dark` | `#04233f` | `rgb(4, 35, 63)` | `hsl(208, 88%, 13%)` |
| ![](https://singlecolorimage.com/get/00030e/20x20) | Ultra Dark | `--mmp-ui-blue-ultra-dark` | `#00030e` | `rgb(0, 3, 14)` | `hsl(227, 100%, 3%)` |

## MMP Gold Shade System
| Swatch | Weight | CSS Variable | Hex Code | RGB | HSL |
| :---: | :--- | :--- | :--- | :--- | :--- |
| ![](https://singlecolorimage.com/get/ffecbe/20x20) | Ultra Light | `--mmp-gold-ultra-light` | `#ffecbe` | `rgb(255, 236, 190)` | `hsl(42, 100%, 87%)` |
| ![](https://singlecolorimage.com/get/eac986/20x20) | Light | `--mmp-gold-light` | `#eac986` | `rgb(234, 201, 134)` | `hsl(40, 71%, 72%)` |
| ![](https://singlecolorimage.com/get/aa8a48/20x20) | Semi Light | `--mmp-gold-semi-light` | `#aa8a48` | `rgb(170, 138, 72)` | `hsl(40, 41%, 47%)` |
| ![](https://singlecolorimage.com/get/c9a967/20x20) | **Main** | `--mmp-gold` | `#c9a967` | `rgb(201, 169, 103)` | `hsl(40, 49%, 60%)` |
| ![](https://singlecolorimage.com/get/eecd8a/20x20) | Hover | `--mmp-gold-hover` | `#eecd8a` | `rgb(238, 205, 138)` | `hsl(40, 75%, 74%)` |
| ![](https://singlecolorimage.com/get/4e3600/20x20) | Semi Dark | `--mmp-gold-semi-dark` | `#4e3600` | `rgb(78, 54, 0)` | `hsl(42, 100%, 15%)` |
| ![](https://singlecolorimage.com/get/2f1e00/20x20) | Dark | `--mmp-gold-dark` | `#2f1e00` | `rgb(47, 30, 0)` | `hsl(38, 100%, 9%)` |
| ![](https://singlecolorimage.com/get/060300/20x20) | Ultra Dark | `--mmp-gold-ultra-dark` | `#060300` | `rgb(6, 3, 0)` | `hsl(30, 100%, 1%)` |

## MMP UI Green Shade System
| Swatch | Weight | CSS Variable | Hex Code | RGB | HSL |
| :---: | :--- | :--- | :--- | :--- | :--- |
| ![](https://singlecolorimage.com/get/7a9d8e/20x20) | Ultra Light | `--mmp-ui-green-ultra-light` | `#7a9d8e` | `rgb(122, 157, 142)` | `hsl(154, 15%, 55%)` |
| ![](https://singlecolorimage.com/get/b3d8c8/20x20) | Light | `--mmp-ui-green-light` | `#b3d8c8` | `rgb(179, 216, 200)` | `hsl(154, 33%, 77%)` |
| ![](https://singlecolorimage.com/get/759889/20x20) | Semi Light | `--mmp-ui-green-semi-light` | `#759889` | `rgb(117, 152, 137)` | `hsl(154, 13%, 53%)` |
| ![](https://singlecolorimage.com/get/7a9d8e/20x20) | **Main** | `--mmp-ui-green` | `#7a9d8e` | `rgb(122, 157, 142)` | `hsl(154, 15%, 55%)` |
| ![](https://singlecolorimage.com/get/98bcad/20x20) | Hover | `--mmp-ui-green-hover` | `#98bcad` | `rgb(152, 188, 173)` | `hsl(155, 21%, 67%)` |
| ![](https://singlecolorimage.com/get/214236/20x20) | Semi Dark | `--mmp-ui-green-semi-dark` | `#214236` | `rgb(33, 66, 54)` | `hsl(158, 33%, 19%)` |
| ![](https://singlecolorimage.com/get/06281d/20x20) | Dark | `--mmp-ui-green-dark` | `#06281d` | `rgb(6, 40, 29)` | `hsl(161, 74%, 9%)` |
| ![](https://singlecolorimage.com/get/000502/20x20) | Ultra Dark | `--mmp-ui-green-ultra-dark` | `#000502` | `rgb(0, 5, 2)` | `hsl(144, 100%, 1%)` |

## MMP Off-White Shade System
| Swatch | Weight | CSS Variable | Hex Code | RGB | HSL |
| :---: | :--- | :--- | :--- | :--- | :--- |
| ![](https://singlecolorimage.com/get/fcfcfc/20x20) | Ultra Light | `--mmp-offwhite-ultra-light` | `#fcfcfc` | `rgb(252, 252, 252)` | `hsl(0, 0%, 99%)` |
| ![](https://singlecolorimage.com/get/fafafa/20x20) | Light | `--mmp-offwhite-light` | `#fafafa` | `rgb(250, 250, 250)` | `hsl(0, 0%, 98%)` |
| ![](https://singlecolorimage.com/get/f9f9f9/20x20) | Semi Light | `--mmp-offwhite-semi-light` | `#f9f9f9` | `rgb(249, 249, 249)` | `hsl(0, 0%, 98%)` |
| ![](https://singlecolorimage.com/get/f8f8f8/20x20) | **Main** | `--mmp-offwhite` | `#f8f8f8` | `rgb(248, 248, 248)` | `hsl(0, 0%, 97%)` |
| ![](https://singlecolorimage.com/get/f2f2f2/20x20) | Hover | `--mmp-offwhite-hover` | `#f2f2f2` | `rgb(242, 242, 242)` | `hsl(0, 0%, 95%)` |
| ![](https://singlecolorimage.com/get/e6e6e6/20x20) | Semi Dark | `--mmp-offwhite-semi-dark` | `#e6e6e6` | `rgb(230, 230, 230)` | `hsl(0, 0%, 90%)` |
| ![](https://singlecolorimage.com/get/ebebeb/20x20) | Dark | `--mmp-offwhite-dark` | `#ebebeb` | `rgb(235, 235, 235)` | `hsl(0, 0%, 92%)` |
| ![](https://singlecolorimage.com/get/bfbfbf/20x20) | Ultra Dark | `--mmp-offwhite-ultra-dark` | `#bfbfbf` | `rgb(191, 191, 191)` | `hsl(0, 0%, 75%)` |

## MMP Gray Shade System
| Swatch | Weight | CSS Variable | Hex Code | RGB | HSL |
| :---: | :--- | :--- | :--- | :--- | :--- |
| ![](https://singlecolorimage.com/get/f2f2f3/20x20) | Ultra Light | `--mmp-gray-ultra-light` | `#f2f2f3` | `rgb(242, 242, 243)` | `hsl(240, 3%, 95%)` |
| ![](https://singlecolorimage.com/get/d9d8db/20x20) | Light | `--mmp-gray-light` | `#d9d8db` | `rgb(217, 216, 219)` | `hsl(260, 3%, 85%)` |
| ![](https://singlecolorimage.com/get/c1c0c4/20x20) | Semi Light | `--mmp-gray-semi-light` | `#c1c0c4` | `rgb(193, 192, 196)` | `hsl(255, 3%, 76%)` |
| ![](https://singlecolorimage.com/get/9f9ea5/20x20) | **Main** | `--mmp-gray` | `#9f9ea5` | `rgb(159, 158, 165)` | `hsl(249, 4%, 63%)` |
| ![](https://singlecolorimage.com/get/949399/20x20) | Hover | `--mmp-gray-hover` | `#949399` | `rgb(148, 147, 153)` | `hsl(250, 3%, 59%)` |
| ![](https://singlecolorimage.com/get/717077/20x20) | Semi Dark | `--mmp-gray-semi-dark` | `#717077` | `rgb(113, 112, 119)` | `hsl(250, 3%, 45%)` |
| ![](https://singlecolorimage.com/get/4d4c4f/20x20) | Dark | `--mmp-gray-dark` | `#4d4c4f` | `rgb(77, 76, 79)` | `hsl(260, 2%, 30%)` |
| ![](https://singlecolorimage.com/get/262527/20x20) | Ultra Dark | `--mmp-gray-ultra-dark` | `#262527` | `rgb(38, 37, 39)` | `hsl(270, 3%, 15%)` |

---

## Rotary International

### Rotary International Official Palette
Used for Rotary-specific components and licensed vendor materials.

| Swatch | Color Name | CSS Variable | Hex Code | RGB | HSL |
| :---: | :--- | :--- | :--- | :--- | :--- |
| ![](https://singlecolorimage.com/get/17458f/20x20) | Royal Blue | `--rotary-royal-blue` | `#17458f` | `rgb(23, 69, 143)` | `hsl(217, 72%, 33%)` |
| ![](https://singlecolorimage.com/get/f7a81b/20x20) | Gold | `--rotary-gold` | `#f7a81b` | `rgb(247, 168, 27)` | `hsl(38, 93%, 54%)` |
| ![](https://singlecolorimage.com/get/0069c8/20x20) | Azure | `--azure` | `#0069c8` | `rgb(0, 105, 200)` | `hsl(208, 100%, 39%)` |
| ![](https://singlecolorimage.com/get/00a2e0/20x20) | Sky Blue | `--sky-blue` | `#00a2e0` | `rgb(0, 162, 224)` | `hsl(197, 100%, 44%)` |
| ![](https://singlecolorimage.com/get/d41367/20x20) | Cranberry | `--cranberry` | `#d41367` | `rgb(212, 19, 103)` | `hsl(334, 84%, 45%)` |
| ![](https://singlecolorimage.com/get/e02927/20x20) | Cardinal | `--cardinal` | `#e02927` | `rgb(224, 41, 39)` | `hsl(1, 74%, 52%)` |
| ![](https://singlecolorimage.com/get/00adbb/20x20) | Turquoise | `--turquoise` | `#00adbb` | `rgb(0, 173, 187)` | `hsl(184, 100%, 37%)` |
| ![](https://singlecolorimage.com/get/ff7600/20x20) | Orange | `--orange` | `#ff7600` | `rgb(255, 118, 0)` | `hsl(28, 100%, 50%)` |
| ![](https://singlecolorimage.com/get/901f93/20x20) | Violet | `--violet` | `#901f93` | `rgb(144, 31, 147)` | `hsl(299, 65%, 35%)` |
| ![](https://singlecolorimage.com/get/019739/20x20) | Grass | `--grass` | `#019739` | `rgb(1, 151, 57)` | `hsl(142, 99%, 30%)` |
| ![](https://singlecolorimage.com/get/b9d9eb/20x20) | Powder Blue | `--powder-blue` | `#b9d9eb` | `rgb(185, 217, 235)` | `hsl(202, 54%, 82%)` |
| ![](https://singlecolorimage.com/get/a7aca2/20x20) | Moss | `--moss` | `#a7aca2` | `rgb(167, 172, 162)` | `hsl(90, 6%, 65%)` |
| ![](https://singlecolorimage.com/get/c6bcd0/20x20) | Lavender | `--lavender` | `#c6bcd0` | `rgb(198, 188, 208)` | `hsl(270, 18%, 78%)` |
| ![](https://singlecolorimage.com/get/d9c89e/20x20) | Taupe | `--taupe` | `#d9c89e` | `rgb(217, 200, 158)` | `hsl(43, 44%, 74%)` |
| ![](https://singlecolorimage.com/get/9ba4b4/20x20) | Mist | `--mist` | `#9ba4b4` | `rgb(155, 164, 180)` | `hsl(218, 15%, 66%)` |
| ![](https://singlecolorimage.com/get/657f99/20x20) | Slate | `--slate` | `#657f99` | `rgb(101, 127, 153)` | `hsl(210, 20%, 50%)` |
| ![](https://singlecolorimage.com/get/54565a/20x20) | Charcoal | `--charcoal` | `#54565a` | `rgb(84, 86, 90)` | `hsl(220, 3%, 34%)` |
| ![](https://singlecolorimage.com/get/898a8d/20x20) | Pewter | `--pewter` | `#898a8d` | `rgb(137, 138, 141)` | `hsl(225, 2%, 55%)` |
| ![](https://singlecolorimage.com/get/b1b1b1/20x20) | Smoke | `--smoke` | `#b1b1b1` | `rgb(177, 177, 177)` | `hsl(0, 0%, 69%)` |
| ![](https://singlecolorimage.com/get/d0cfcd/20x20) | Silver | `--silver` | `#d0cfcd` | `rgb(208, 207, 205)` | `hsl(40, 3%, 81%)` |
| ![](https://singlecolorimage.com/get/ffffff/20x20) | White | `--white` | `#ffffff` | `rgb(255, 255, 255)` | `hsl(0, 0%, 100%)` |
| ![](https://singlecolorimage.com/get/000000/20x20) | Black | `--black` | `#000000` | `rgb(0, 0, 0)` | `hsl(0, 0%, 0%)` |
| ![](https://singlecolorimage.com/get/7a6e66/20x20) | Storm | `--storm` | `#7a6e66` | `rgb(122, 110, 102)` | `hsl(24, 9%, 44%)` |
| ![](https://singlecolorimage.com/get/968b83/20x20) | Ash | `--ash` | `#968b83` | `rgb(150, 139, 131)` | `hsl(25, 9%, 55%)` |
| ![](https://singlecolorimage.com/get/bfb7b0/20x20) | Platinum | `--platinum` | `#bfb7b0` | `rgb(191, 183, 176)` | `hsl(28, 11%, 72%)` |
| ![](https://singlecolorimage.com/get/d6d1ca/20x20) | Cloud | `--cloud` | `#d6d1ca` | `rgb(214, 209, 202)` | `hsl(35, 13%, 82%)` |

Rotary International brand colors are provided in this repository **only as a convenience**, and only in the context of Member Minder Pro being a licensed, authorized vendor of Rotary International.

**All Rotary International copyrights and trademarks belong to Rotary International and are used with permission.**

For dedicated Rotary branding (e.g. Rotary logos, Masterbrand, and full Rotary color set), see the [Rotary Brand Assets](https://github.com/memberminderpro/rotary-brand-assets) repository and [Rotary International's Brand Center guidelines](https://brandcenter.rotary.org/en-us/our-brand/brand-elements).

---

## Contributing

We welcome contributions to this repository. If you have suggestions for improvements or want to contribute to the ongoing development of these assets, please follow the process below:

1. **Fork the repository** — Fork the repository to your own GitHub account.

2. **Clone the forked repository** — Clone it to your local machine.

   ```bash
   git clone https://github.com/your-username/brand-assets.git
   cd brand-assets
   ```

3. **Create a new branch** — Create a branch for your changes.

   ```bash
   git checkout -b your-new-branch-name
   ```

4. **Make your changes** — Implement your changes in your branch.

5. **Commit your changes** — Commit with a clear, descriptive message.

   ```bash
   git commit -m "A brief description of the changes"
   ```

6. **Push to GitHub** — Push your branch to your fork.

   ```bash
   git push origin your-new-branch-name
   ```

7. **Submit a pull request** — Open a pull request against the original repository with a clear description of your changes.

8. **Review and merge** — Maintainers will review your pull request; if appropriate, it will be merged.

We appreciate your efforts to contribute and look forward to collaborating with you.

---

## License, ownership, and attribution

### Member Minder Pro brand assets

The Member Minder Pro brand assets in this repository (logos, icons, color definitions, and related materials) are owned by **Member Minder Pro, LLC**. Their use should align with the purpose of this repository and with any usage guidelines provided here or by Member Minder Pro.

### Rotary International assets

Rotary International brand elements (e.g. colors, and any Rotary-specific assets if added) are owned by Rotary International and are used here with permission. See the [Rotary International](#rotary-international) section above.

### Code and implementation

The code and implementation in this repository (e.g. CSS variables, file structure, and tooling) have been created by [Member Minder Pro, LLC](https://memberminderpro.com). This work is released as open source and is available for use under a fair use license with attribution.

### License

This project is licensed under a modified MIT License: free use, modification, and distribution are permitted, provided that use of the assets or code retains attribution to Member Minder Pro. Any distribution of modified versions should be under the same or a similar license and include proper attribution.

By using these assets and code, you agree to adhere to these terms and to credit Member Minder Pro in any derivative works or distributions.

#### How to attribute

When using assets or code from this repository, please include attribution such as:

"Brand assets and implementation provided by [Member Minder Pro, LLC](https://memberminderpro.com), used under MIT License."

#### Modifications and sharing

You may modify and share the assets and code in this repository, provided that any distributed versions include proper attribution to [Member Minder Pro, LLC](https://memberminderpro.com) and are released under the same or a similar open-source license.

---

## About us

[Member Minder Pro](https://www.memberminderpro.com) is an official [Rotary International Licensee](https://my.rotary.org/en/my-rotary/community-marketplace/club-management-systems-and-website-providers), and is dedicated to providing innovative solutions such as [DACdb](https://www.dacdb.org/) — tailored specifically for organizations within Rotary International. Our focus is on developing user-friendly, efficient, and effective digital tools and resources.

> Built By Rotarians For Rotarians

We believe in the power of community and technology to make a positive impact. Our team is committed to supporting organizations in streamlining their processes and enhancing their digital presence.

**Connect with us:**

- Visit our website: [Member Minder Pro, LLC](https://www.memberminderpro.com)
- Follow us on Twitter: [@MemberMinderPro](https://twitter.com/MemberMinderPro)
- Like us on Facebook: [Member Minder Pro on Facebook](https://www.facebook.com/MemberMinderPro)
- Connect with us on LinkedIn: [Member Minder Pro on LinkedIn](https://www.linkedin.com/company/memberminderpro/)

For more information about our services and how we can assist your organization, please visit our website or contact us through our social media channels.
