# Roboto Font Files

This directory contains links and information for downloading the Roboto font.

## About Roboto

Roboto is a versatile geometric sans-serif typeface family designed by Christian Robertson for Google.
It's one of the most widely used web fonts globally, perfect for any kind of design application.

## Official Sources

**Google Fonts:** https://fonts.google.com/specimen/Roboto
**GitHub Repository:** https://github.com/google/fonts/tree/main/apache/roboto

## Direct Download Links

### Regular Weight (400)

- **TTF Format:** https://github.com/google/fonts/blob/main/apache/roboto/Roboto-Regular.ttf?raw=true
- **WOFF2 Format:** https://fonts.gstatic.com/s/roboto/v30/KFOmCnqEu92Fr1Mu4mxP.woff2
- **WOFF Format:** https://fonts.gstatic.com/s/roboto/v30/KFOmCnqEu92Fr1MmWUlfBBc4.woff

### Light Weight (300)

- **TTF Format:** https://github.com/google/fonts/blob/main/apache/roboto/Roboto-Light.ttf?raw=true
- **WOFF2 Format:** https://fonts.gstatic.com/s/roboto/v30/KFOkCnqEu92Fr1MmYUtfBBc-.woff2

### Medium Weight (500)

- **TTF Format:** https://github.com/google/fonts/blob/main/apache/roboto/Roboto-Medium.ttf?raw=true
- **WOFF2 Format:** https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmEU9fBBc-.woff2

### Bold Weight (700)

- **TTF Format:** https://github.com/google/fonts/blob/main/apache/roboto/Roboto-Bold.ttf?raw=true
- **WOFF2 Format:** https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmWUlfCRc_.woff2
- **WOFF Format:** https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmWUlfCBc4.woff

### Black Weight (900)

- **TTF Format:** https://github.com/google/fonts/blob/main/apache/roboto/Roboto-Black.ttf?raw=true
- **WOFF2 Format:** https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmYUtfCRc-.woff2

## Download All Formats at Once

### Option 1: From Google Fonts
1. Visit https://fonts.google.com/specimen/Roboto
2. Click "Download family"
3. Get all weights and styles

### Option 2: From GitHub
All TTF files: https://github.com/google/fonts/tree/main/apache/roboto

## Installation

### For Web Use

Copy WOFF2 files to your web server:
```css
@font-face {
  font-family: 'Roboto';
  font-weight: 400;
  src: url('/fonts/roboto/Roboto-Regular.woff2') format('woff2'),
       url('/fonts/roboto/Roboto-Regular.woff') format('woff');
  font-display: swap;
}

@font-face {
  font-family: 'Roboto';
  font-weight: 700;
  src: url('/fonts/roboto/Roboto-Bold.woff2') format('woff2'),
       url('/fonts/roboto/Roboto-Bold.woff') format('woff');
  font-display: swap;
}

body {
  font-family: 'Roboto', sans-serif;
}
```

### For Desktop

1. Download TTF files
2. Right-click and select "Install" (Windows) or double-click (macOS/Linux)

## Available Weights

| Weight | Font File |
|--------|-----------|
| 300 | Roboto-Light |
| 400 | Roboto-Regular |
| 500 | Roboto-Medium |
| 700 | Roboto-Bold |
| 900 | Roboto-Black |

Plus Thin (100) available from Google Fonts.

## File Sizes (Approximate)

| Format | Size |
|--------|------|
| TTF | ~90-120 KB per weight |
| WOFF2 | ~50-65 KB per weight |
| WOFF | ~80-100 KB per weight |

WOFF2 is recommended for web use (best compression).

## License

Roboto is licensed under the **Apache License 2.0**

See the LICENSE file for complete terms.

## Support

- Google Fonts: https://fonts.google.com/specimen/Roboto
- GitHub Repository: https://github.com/google/fonts/tree/main/apache/roboto
- Apache License 2.0: https://www.apache.org/licenses/LICENSE-2.0

## Font Features

- **Geometric design** - Clean, modern look
- **Warm character** - Friendly despite geometric nature
- **Versatile** - Works for headings, body text, UI
- **Professional** - Used by Google and major brands
- **Extensive language support** - Latin, Cyrillic, Greek, etc.

---

**Designed by:** Christian Robertson  
**Maintained by:** Google Inc.  
**License:** Apache License 2.0  
**Last Updated:** 2026-09-01
