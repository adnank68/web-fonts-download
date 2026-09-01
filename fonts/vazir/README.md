# Vazir Font

A clean and modern Persian typeface designed for optimal readability on screens and in print.

## About Vazir

Vazir is a professional Persian sans-serif font created by Saber Rastikerdar. It's specifically designed for Persian text with excellent legibility and modern aesthetic.

## Font Weights Available

- Regular (400)
- Bold (700)

## File Formats

This directory contains Vazir font in multiple formats:

- **TTF** - TrueType format (desktop, print)
- **WOFF** - Web Open Font Format (web, good compression)
- **WOFF2** - Web Open Font Format 2 (web, best compression - recommended)

## Installation

### For Web Use

```css
@font-face {
  font-family: 'Vazir';
  src: url('/fonts/vazir/Vazir.woff2') format('woff2'),
       url('/fonts/vazir/Vazir.woff') format('woff'),
       url('/fonts/vazir/Vazir.ttf') format('truetype');
  font-display: swap;
}

body {
  font-family: 'Vazir', sans-serif;
}
```

### For Desktop/Applications

Download the TTF file and install on your system:
- **Windows:** Right-click → Install
- **macOS:** Double-click → Install Font
- **Linux:** Copy to ~/.local/share/fonts/ → Run `fc-cache`

## Usage Examples

### HTML with Persian Text

```html
<!DOCTYPE html>
<html dir="rtl" lang="fa">
<head>
  <meta charset="UTF-8">
  <style>
    @font-face {
      font-family: 'Vazir';
      src: url('/fonts/vazir/Vazir.woff2') format('woff2');
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

## Technical Details

- **Creator:** Saber Rastikerdar
- **License:** SIL Open Font License (OFL) v1.1
- **Repository:** https://github.com/rastikerdar/vazir-font
- **Language Support:** Persian, Arabic, English
- **Character Set:** Extensive Persian and Arabic character coverage

## Performance Optimization

For web use, follow these best practices:

1. **Use WOFF2** - Smallest file size
2. **Preload critical weights:**
   ```html
   <link rel="preload" href="/fonts/vazir/Vazir.woff2" as="font" type="font/woff2" crossorigin>
   ```

3. **Font display strategy:**
   ```css
   @font-face {
     font-family: 'Vazir';
     src: url('/fonts/vazir/Vazir.woff2') format('woff2');
     font-display: swap; /* Show fallback immediately */
   }
   ```

4. **Subsetting** - If you only need certain characters, subset the font to reduce file size

## File Sizes

| Format | File Size |
|--------|-----------|
| Vazir-Regular.woff2 | ~45 KB |
| Vazir-Regular.woff | ~65 KB |
| Vazir-Regular.ttf | ~95 KB |
| Vazir-Bold.woff2 | ~48 KB |
| Vazir-Bold.woff | ~68 KB |
| Vazir-Bold.ttf | ~100 KB |

## Compatibility

- **Web Browsers:** All modern browsers (Chrome, Firefox, Safari, Edge)
- **Desktop:** Windows, macOS, Linux
- **Mobile:** iOS, Android
- **Design Software:** Adobe Creative Suite, Figma, Sketch, etc.

## License

Vazir is licensed under the **SIL Open Font License (OFL) v1.1**

You can:
- ✅ Use for personal and commercial projects
- ✅ Embed in websites
- ✅ Use in applications
- ✅ Modify and redistribute (with attribution)

You must:
- ✅ Include the LICENSE file
- ✅ Credit Saber Rastikerdar
- ✅ Not claim ownership

See `LICENSE` file for complete terms.

## Resources

- **Original Repository:** https://github.com/rastikerdar/vazir-font
- **SIL OFL:** https://scripts.sil.org/OFL
- **Font Website:** https://rastikerdar.github.io/vazir-font/

## Support

For issues or questions:
1. Check the main README.md
2. Visit the original repository
3. Open an issue on GitHub

---

**Created by:** Saber Rastikerdar  
**Licensed under:** SIL Open Font License v1.1  
**Last Updated:** 2026-09-01
