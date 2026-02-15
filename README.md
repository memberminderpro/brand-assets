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

## MemberMinder Pro primary color palette

Primary palette: the **main shade** of each MMP color system (one per family). Full shade systems (ultra-light, light, semi-light, dark, hover, etc.) are defined in `css/colors.css`.

| Color        | Role        | Hex       | RGB             | CSS variable   |
| ------------ | ----------- | --------- | --------------- | --------------- |
| MMP Blue     | Logo        | `#1e224e` | 30, 34, 78      | `--mmp-blue`   |
| MMP Red      | Logo        | `#841c30` | 132, 28, 48     | `--mmp-red`    |
| MMP UI Blue  | Primary     | `#8dafd3` | 141, 175, 211   | `--mmp-ui-blue`|
| MMP UI Gold  | Secondary   | `#c9a967` | 201, 169, 103   | `--mmp-gold`   |
| MMP UI Green | Tertiary    | `#7a9d8e` | 122, 157, 142   | `--mmp-ui-green`|
| MMP Off-White| Base        | `#f8f8f8` | 248, 248, 248   | `--mmp-offwhite`|
| MMP Gray     | Neutral     | `#9f9ea5` | 159, 158, 165   | `--mmp-gray`   |

---

## Rotary International

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
