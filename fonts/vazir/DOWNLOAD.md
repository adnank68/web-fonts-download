# Vazir Font Files

This directory contains links and information for downloading the Vazir font.

## About Vazir

Vazir is a professional Persian (Farsi) sans-serif typeface created by Saber Rastikerdar.
It's designed for optimal readability on screens and in print, with excellent support for Persian and Arabic text.

## Official Source

**Main Repository:** https://github.com/rastikerdar/vazir-font

## Direct Download Links

### Regular Weight (400)

- **TTF Format:** https://rastikerdar.github.io/vazir-font/dist/Vazir-Regular.ttf
- **WOFF Format:** https://rastikerdar.github.io/vazir-font/dist/Vazir-Regular.woff
- **WOFF2 Format:** https://rastikerdar.github.io/vazir-font/dist/Vazir-Regular.woff2

### Bold Weight (700)

- **TTF Format:** https://rastikerdar.github.io/vazir-font/dist/Vazir-Bold.ttf
- **WOFF Format:** https://rastikerdar.github.io/vazir-font/dist/Vazir-Bold.woff
- **WOFF2 Format:** https://rastikerdar.github.io/vazir-font/dist/Vazir-Bold.woff2

## Download All Formats at Once

Download the complete Vazir font package from the official releases:
**https://github.com/rastikerdar/vazir-font/releases/latest**

This includes:
- All weights (Regular, Bold)
- All formats (TTF, WOFF, WOFF2)
- LICENSE and documentation

## Installation

### For Web Use

Copy WOFF2 files to your web server:
```css
@font-face {
  font-family: 'Vazir';
  src: url('/fonts/vazir/Vazir.woff2') format('woff2'),
       url('/fonts/vazir/Vazir.woff') format('woff');
  font-display: swap;
}

@font-face {
  font-family: 'Vazir';
  font-weight: bold;
  src: url('/fonts/vazir/Vazir-Bold.woff2') format('woff2'),
       url('/fonts/vazir/Vazir-Bold.woff') format('woff');
  font-display: swap;
}

body {
  font-family: 'Vazir', sans-serif;
}
```

### For Desktop

1. Download TTF files
2. Right-click and select "Install" (Windows) or double-click (macOS/Linux)

## Font Files Information

| File | Format | Usage |
|------|--------|-------|
| Vazir-Regular | TTF, WOFF, WOFF2 | Regular weight for body text |
| Vazir-Bold | TTF, WOFF, WOFF2 | Bold weight for headings |

## License

Vazir is licensed under the **SIL Open Font License (OFL) v1.1**

See the LICENSE file for complete terms.

## Support

- Original Font: https://github.com/rastikerdar/vazir-font
- SIL OFL: https://scripts.sil.org/OFL
- Font Demo: https://rastikerdar.github.io/vazir-font/

---

**Creator:** Saber Rastikerdar  
**License:** SIL Open Font License v1.1  
**Language:** Persian, Arabic, English