# Web Fonts Download

A lightweight collection of the most popular and useful open-source web fonts ready for download and integration into your projects.

## Overview

This repository provides easy access to carefully selected open-source web fonts. Currently featuring:
- **Vazir** - Professional Persian font
- **Roboto** - World's most popular web font (by Google)

All fonts are open-source, legally free to use, and can be used for both personal and commercial projects.

## Available Fonts

### Persian/Arabic Fonts

#### Vazir
A clean and modern Persian sans-serif typeface designed for optimal readability on screens and in print.

- **Creator:** Saber Rastikerdar
- **License:** SIL Open Font License (OFL) v1.1
- **Weights:** Regular, Bold
- **Formats:** TTF, WOFF, WOFF2
- **Use Cases:** Websites, applications, print materials
- **Repository:** https://github.com/rastikerdar/vazir-font

**Features:**
- Excellent legibility for Persian text
- Modern, professional appearance
- Optimized for screen display
- Supports Arabic and English characters

📁 **Location:** `fonts/vazir/`
📖 **Documentation:** `fonts/vazir/README.md`

---

### English/Latin Fonts

#### Roboto
A versatile geometric sans-serif typeface family designed by Google. One of the most widely used web fonts globally with excellent versatility across all design applications.

- **Creator:** Christian Robertson (Google Inc.)
- **License:** Apache License 2.0
- **Weights:** Thin, Light, Regular, Medium, Bold, Black
- **Formats:** TTF, WOFF, WOFF2
- **Use Cases:** Web, mobile apps, desktop applications, print
- **Repository:** https://github.com/google/roboto
- **Google Fonts:** https://fonts.google.com/specimen/Roboto

**Features:**
- Geometric design with warm character
- Six weight options for maximum flexibility
- Excellent readability at any size
- Perfect for both headings and body text
- Used by Google and thousands of major brands

**Why Roboto?**
- ✅ Most popular web font worldwide
- ✅ Extensive language support
- ✅ Professional and modern appearance
- ✅ Proven track record in web design

📁 **Location:** `fonts/roboto/`
📖 **Documentation:** `fonts/roboto/README.md`

---

## How to Use

### 1. Download Fonts

Navigate to the `fonts/` directory and download the font format you need:

**For Web (Recommended):**
- **WOFF2** - Best compression, excellent browser support (use this!)
- **WOFF** - Good compatibility with older browsers

**For Desktop/Print:**
- **TTF** - Standard format for desktop applications and print

### 2. Web Implementation

Add fonts to your CSS:

```css
/* Roboto Example */
@font-face {
  font-family: 'Roboto';
  font-weight: 400;
  src: url('/fonts/roboto/Roboto-Regular.woff2') format('woff2'),
       url('/fonts/roboto/Roboto-Regular.woff') format('woff'),
       url('/fonts/roboto/Roboto-Regular.ttf') format('truetype');
  font-display: swap;
}

@font-face {
  font-family: 'Roboto';
  font-weight: 700;
  src: url('/fonts/roboto/Roboto-Bold.woff2') format('woff2'),
       url('/fonts/roboto/Roboto-Bold.woff') format('woff'),
       url('/fonts/roboto/Roboto-Bold.ttf') format('truetype');
  font-display: swap;
}

body {
  font-family: 'Roboto', sans-serif;
}

strong {
  font-weight: 700;
}
```

### 3. HTML Implementation - Preload Fonts

For better performance, preload critical fonts:

```html
<link rel="preload" href="/fonts/roboto/Roboto-Regular.woff2" as="font" type="font/woff2" crossorigin>
<link rel="preload" href="/fonts/roboto/Roboto-Bold.woff2" as="font" type="font/woff2" crossorigin>
```

### 4. Persian Text Example (Vazir)

```html
<!DOCTYPE html>
<html dir="rtl" lang="fa">
<head>
  <meta charset="UTF-8">
  <style>
    @font-face {
      font-family: 'Vazir';
      src: url('/fonts/vazir/Vazir.woff2') format('woff2');
      font-display: swap;
    }
    body {
      font-family: 'Vazir', sans-serif;
    }
  </style>
</head>
<body>
  <h1>سلام دنیا</h1>
  <p>این یک نمونه از فونت وزیر است.</p>
</body>
</html>
```

## Font Licenses

### Legal Status: ✅ FULLY LEGAL

All fonts in this repository are open-source and distributed under permissive licenses:

#### Vazir Font
- **License:** SIL Open Font License (OFL) v1.1
- **Status:** Free for personal and commercial use
- **Permissions:** Use, modify, redistribute (with attribution)

#### Roboto Font
- **License:** Apache License 2.0
- **Status:** Free for personal and commercial use
- **Permissions:** Use, modify, redistribute (with attribution)

### What You Can Do ✅

- ✅ Use on websites (commercial and personal)
- ✅ Embed in web applications
- ✅ Use in desktop and mobile applications
- ✅ Use in print materials and designs
- ✅ Modify fonts (subset, optimize, etc.)
- ✅ Redistribute with proper attribution
- ✅ Use commercially without paying royalties

### What You Must Do ✅

- ✅ Include the LICENSE file with distributions
- ✅ Credit the original font creators
- ✅ Clearly indicate any modifications made
- ✅ Not claim ownership of the original fonts

### What You Cannot Do ❌

- ❌ Sell the fonts as standalone products
- ❌ Remove creator attribution
- ❌ Claim to have created the fonts
- ❌ Redistribute without including the license files

**For complete legal details, see `LEGAL.md`**

## File Organization

```
web-fonts-download/
├── fonts/
│   ├── vazir/
│   │   ├── Vazir.ttf
│   │   ├── Vazir.woff
│   │   ├── Vazir.woff2
│   │   ├── Vazir-Bold.ttf
│   │   ├── Vazir-Bold.woff
│   │   ├── Vazir-Bold.woff2
│   │   ├── LICENSE
│   │   └── README.md
│   │
│   └── roboto/
│       ├── Roboto-Thin.ttf
│       ├── Roboto-Light.ttf
│       ├── Roboto-Regular.ttf
│       ├── Roboto-Medium.ttf
│       ├── Roboto-Bold.ttf
│       ├── Roboto-Black.ttf
│       ├── [WOFF versions]
│       ├── [WOFF2 versions]
│       ├── LICENSE
│       └── README.md
├── README.md (this file)
├── LEGAL.md (legal information)
├── CREDITS.md (attribution information)
├── CONTRIBUTING.md (contribution guidelines)
├── FONTS-DIRECTORY.md (directory structure)
├── package.json (project metadata)
└── index.html (interactive landing page)
```

## Performance Tips

### For Web Performance

1. **Use WOFF2 Format** - Smallest file size, excellent browser support
2. **Preload Critical Fonts** - Use `rel="preload"` for above-the-fold fonts
3. **Font Display Strategy** - Use `font-display: swap` to avoid blocking
4. **Only Load Weights You Use** - Don't load all weights if you only need regular and bold
5. **Subsetting** - For large character sets, consider subsetting to essential characters

### CSS Example with Performance Best Practices

```css
@font-face {
  font-family: 'Roboto';
  font-weight: 400;
  src: url('/fonts/roboto/Roboto-Regular.woff2') format('woff2'),
       url('/fonts/roboto/Roboto-Regular.woff') format('woff');
  font-display: swap; /* Ensures text is visible while font loads */
}

@font-face {
  font-family: 'Roboto';
  font-weight: 700;
  src: url('/fonts/roboto/Roboto-Bold.woff2') format('woff2'),
       url('/fonts/roboto/Roboto-Bold.woff') format('woff');
  font-display: swap;
}

body {
  font-family: 'Roboto', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
}
```

## File Sizes Reference

| Font | Format | Size |
|------|--------|------|
| Vazir Regular | WOFF2 | ~45 KB |
| Vazir Bold | WOFF2 | ~48 KB |
| Roboto Regular | WOFF2 | ~55 KB |
| Roboto Bold | WOFF2 | ~58 KB |
| Roboto Light | WOFF2 | ~52 KB |

## Quick Links

- 📖 **Full Documentation:** See individual font README files in `fonts/[fontname]/README.md`
- ⚖️ **Legal Information:** See `LEGAL.md`
- 🎨 **Attribution & Credits:** See `CREDITS.md`
- 🤝 **Contributing:** See `CONTRIBUTING.md`
- 🌐 **Interactive Demo:** See `index.html`
- 📁 **Directory Guide:** See `FONTS-DIRECTORY.md`

## Resources

- [Google Fonts - Roboto](https://fonts.google.com/specimen/Roboto)
- [Vazir Font Repository](https://github.com/rastikerdar/vazir-font)
- [SIL Open Font License](https://scripts.sil.org/OFL)
- [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)
- [MDN @font-face Documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/@font-face)
- [Font Loading Best Practices](https://web.dev/font-best-practices/)

## Contributing

We welcome contributions! To add more open-source fonts:

1. Fork the repository
2. Add font files to `fonts/[fontname]/`
3. Include LICENSE file
4. Add README.md documentation
5. Update this README
6. Create a pull request

See `CONTRIBUTING.md` for detailed guidelines.

## License

**This repository:** MIT License

**Fonts:** 
- Vazir: SIL Open Font License v1.1
- Roboto: Apache License 2.0

See individual font directories for complete license information.

## Support & Questions

- 📚 Read the `README.md` files in each font directory
- ⚖️ Check `LEGAL.md` for legal questions
- 🤝 Open an issue on GitHub
- 📖 Visit the official font repositories

## Changelog

### Version 1.0.0 (2026-09-01)
- Initial release
- Added Vazir font (Persian)
- Added Roboto font (English)
- Complete documentation and legal information
- Interactive landing page

---

## Summary

**Web Fonts Download** provides two essential open-source fonts:

1. **Vazir** - Perfect for Persian language websites and applications
2. **Roboto** - The world's most popular web font by Google

Both are:
- ✅ Completely free
- ✅ Open-source and legally distributable
- ✅ Suitable for commercial projects
- ✅ Well-documented and supported
- ✅ Optimized for web and print

**Get started today by downloading your preferred font and following the implementation guides above!**

---

**Last Updated:** 2026-09-01  
**Version:** 1.0.0  
**Repository:** https://github.com/adnank68/web-fonts-download

Enjoy using these beautiful fonts in your projects! 🎨
