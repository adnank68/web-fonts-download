# Roboto Font

A versatile and popular sans-serif typeface family designed by Christian Robertson for Google. Roboto is one of the most widely used web fonts globally.

## About Roboto

Roboto is a geometric sans-serif typeface that works well for any kind of design. The regular character forms are quite geometric, while the italics are more dramatic. The overall result is a font with excellent legibility for any size.

## Font Weights Available

- Thin (100)
- Light (300)
- Regular (400)
- Medium (500)
- Bold (700)
- Black (900)

## File Formats

This directory contains Roboto font in multiple formats:

- **TTF** - TrueType format (desktop, print)
- **WOFF** - Web Open Font Format (web, good compression)
- **WOFF2** - Web Open Font Format 2 (web, best compression - recommended)

## Installation

### For Web Use

```css
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
  font-weight: 400;
}

strong, b {
  font-weight: 700;
}

.light {
  font-weight: 300;
}

.medium {
  font-weight: 500;
}

.black {
  font-weight: 900;
}
```

### For Desktop/Applications

Download the TTF file and install on your system:
- **Windows:** Right-click → Install
- **macOS:** Double-click → Install Font
- **Linux:** Copy to ~/.local/share/fonts/ → Run `fc-cache`

## Usage Examples

### Basic HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <style>
    @font-face {
      font-family: 'Roboto';
      src: url('/fonts/roboto/Roboto-Regular.woff2') format('woff2');
    }
    body {
      font-family: 'Roboto', sans-serif;
    }
  </style>
</head>
<body>
  <h1>Welcome to Roboto</h1>
  <p>The quick brown fox jumps over the lazy dog.</p>
</body>
</html>
```

### Multiple Weights

```html
<style>
  @font-face {
    font-family: 'Roboto';
    font-weight: 300;
    src: url('/fonts/roboto/Roboto-Light.woff2') format('woff2');
  }
  
  @font-face {
    font-family: 'Roboto';
    font-weight: 400;
    src: url('/fonts/roboto/Roboto-Regular.woff2') format('woff2');
  }
  
  @font-face {
    font-family: 'Roboto';
    font-weight: 700;
    src: url('/fonts/roboto/Roboto-Bold.woff2') format('woff2');
  }

  body { font-family: 'Roboto', sans-serif; }
  .light { font-weight: 300; }
  .bold { font-weight: 700; }
</style>
```

## Technical Details

- **Creator:** Christian Robertson
- **Maintained by:** Google Inc.
- **License:** Apache License 2.0
- **Repository:** https://github.com/google/roboto
- **Language Support:** Extensive Latin character coverage
- **Design Category:** Geometric Sans-Serif

## Performance Optimization

For web use, follow these best practices:

1. **Use WOFF2** - Smallest file size
2. **Preload critical weights:**
   ```html
   <link rel="preload" href="/fonts/roboto/Roboto-Regular.woff2" as="font" type="font/woff2" crossorigin>
   <link rel="preload" href="/fonts/roboto/Roboto-Bold.woff2" as="font" type="font/woff2" crossorigin>
   ```

3. **Font display strategy:**
   ```css
   @font-face {
     font-family: 'Roboto';
     src: url('/fonts/roboto/Roboto-Regular.woff2') format('woff2');
     font-display: swap; /* Show fallback immediately */
   }
   ```

4. **Variable Font** - If available, use variable font to load all weights at once with smaller file size

5. **Subsetting** - Only load weights you actually use

## File Sizes

| Font File | Format | File Size |
|-----------|--------|-----------|
| Roboto-Thin | WOFF2 | ~50 KB |
| Roboto-Light | WOFF2 | ~52 KB |
| Roboto-Regular | WOFF2 | ~55 KB |
| Roboto-Medium | WOFF2 | ~55 KB |
| Roboto-Bold | WOFF2 | ~58 KB |
| Roboto-Black | WOFF2 | ~60 KB |

## Design Characteristics

- **Geometric:** Constructed from simple geometric forms
- **Friendly:** Despite its geometric nature, it feels warm and human
- **Universal:** Works equally well in headings and body text
- **Diverse:** Six weights for maximum flexibility
- **Legible:** Excellent readability at all sizes

## Compatibility

- **Web Browsers:** All modern browsers (Chrome, Firefox, Safari, Edge)
- **Mobile Browsers:** iOS Safari, Chrome Android
- **Desktop:** Windows, macOS, Linux
- **Design Software:** Adobe Creative Suite, Figma, Sketch, etc.
- **Email:** Limited support (not recommended for email)

## License

Roboto is licensed under the **Apache License 2.0**

You can:
- ✅ Use for personal and commercial projects
- ✅ Embed in websites
- ✅ Use in applications and software
- ✅ Modify and redistribute (with attribution)

You must:
- ✅ Include the LICENSE file
- ✅ Include NOTICE file with attribution
- ✅ Document any modifications

See `LICENSE` file for complete terms.

## Resources

- **Official Repository:** https://github.com/google/roboto
- **Google Fonts:** https://fonts.google.com/specimen/Roboto
- **Apache License 2.0:** https://www.apache.org/licenses/LICENSE-2.0
- **Roboto Specimen:** https://www.google.com/fonts/specimen/Roboto

## Popular Uses

Roboto is used by:
- Google and all major Google products
- Android operating system
- Thousands of websites globally
- Major brands and applications

## Support

For issues or questions:
1. Check the main README.md
2. Visit the official Google Roboto repository
3. Check Google Fonts documentation
4. Open an issue on GitHub

---

**Designed by:** Christian Robertson  
**Maintained by:** Google Inc.  
**Licensed under:** Apache License 2.0  
**Last Updated:** 2026-09-01
