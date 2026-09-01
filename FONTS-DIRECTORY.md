# Font Directory Structure

This document outlines where each font is stored and how to access the files.

## Directory Layout

```
fonts/
├── vazir/
│   ├── Vazir.ttf
│   ├── Vazir.woff
│   ├── Vazir.woff2
│   ├── Vazir-Bold.ttf
│   ├── Vazir-Bold.woff
│   ├── Vazir-Bold.woff2
│   ├── LICENSE
│   └── README.md
│
├── roboto/
│   ├── Roboto-Thin.ttf
│   ├── Roboto-Light.ttf
│   ├── Roboto-Regular.ttf
│   ├── Roboto-Medium.ttf
│   ├── Roboto-Bold.ttf
│   ├── Roboto-Black.ttf
│   ├── [WOFF versions]
│   ├── [WOFF2 versions]
│   ├── LICENSE
│   └── README.md
│
├── ubuntu/
│   ├── Ubuntu-Light.ttf
│   ├── Ubuntu-Regular.ttf
│   ├── Ubuntu-Medium.ttf
│   ├── Ubuntu-Bold.ttf
│   ├── [WOFF versions]
│   ├── [WOFF2 versions]
│   ├── LICENSE
│   └── README.md
│
├── inter/
│   ├── Inter-Thin.ttf
│   ├── Inter-Light.ttf
│   ├── Inter-Regular.ttf
│   ├── Inter-Medium.ttf
│   ├── Inter-Bold.ttf
│   ├── Inter-Black.ttf
│   ├── [WOFF versions]
│   ├── [WOFF2 versions]
│   ├── LICENSE
│   └── README.md
│
├── lato/
│   ├── Lato-Light.ttf
│   ├── Lato-Regular.ttf
│   ├── Lato-Bold.ttf
│   ├── [WOFF versions]
│   ├── [WOFF2 versions]
│   ├── LICENSE
│   └── README.md
│
└── opensans/
    ├── OpenSans-Light.ttf
    ├── OpenSans-Regular.ttf
    ├── OpenSans-SemiBold.ttf
    ├── OpenSans-Bold.ttf
    ├── [WOFF versions]
    ├── [WOFF2 versions]
    ├── LICENSE
    └── README.md
```

## Font File Naming

### Naming Convention

- **Weight indicators:** Thin, Light, Regular, Medium, Bold, Black, ExtraBold
- **Style indicators:** Italic (only if separate file)
- **Format:** `FontName-Weight.extension`

### Examples

- `Vazir.ttf` - Regular weight
- `Roboto-Bold.ttf` - Bold weight
- `Inter-Light.woff2` - Light weight in WOFF2 format
- `Lato-Regular.woff` - Regular weight in WOFF format

## Accessing Fonts

### From the Web

Self-host fonts on your website:

```css
@font-face {
  font-family: 'Vazir';
  src: url('/fonts/vazir/Vazir.woff2') format('woff2'),
       url('/fonts/vazir/Vazir.woff') format('woff'),
       url('/fonts/vazir/Vazir.ttf') format('truetype');
}

@font-face {
  font-family: 'Vazir';
  font-weight: bold;
  src: url('/fonts/vazir/Vazir-Bold.woff2') format('woff2'),
       url('/fonts/vazir/Vazir-Bold.woff') format('woff'),
       url('/fonts/vazir/Vazir-Bold.ttf') format('truetype');
}

body {
  font-family: 'Vazir', sans-serif;
}

strong {
  font-weight: bold;
}
```

### Direct Download URLs

Access files directly from GitHub:

```
https://raw.githubusercontent.com/adnank68/web-fonts-download/main/fonts/[fontname]/[filename]
```

Examples:
- `https://raw.githubusercontent.com/adnank68/web-fonts-download/main/fonts/vazir/Vazir.woff2`
- `https://raw.githubusercontent.com/adnank68/web-fonts-download/main/fonts/roboto/Roboto-Bold.ttf`

### Clone Repository

Clone the entire project:

```bash
git clone https://github.com/adnank68/web-fonts-download.git
cd web-fonts-download
```

All fonts are in the `fonts/` directory.

## Formats Available

Each font includes multiple formats for different use cases:

### Format Reference Table

| Format | Extension | Best For | Browser Support |
|--------|-----------|----------|-----------------|
| TrueType | .ttf | Desktop, Print, Fallback | All browsers |
| OpenType | .otf | Advanced features | Most browsers |
| WOFF | .woff | Web, good compression | Modern browsers |
| WOFF2 | .woff2 | Web, best compression | Modern browsers |

### Format Recommendations

| Use Case | Recommended Format | Secondary Format |
|----------|-------------------|-----------------|
| Website (web fonts) | WOFF2 | WOFF |
| Desktop Application | TTF | OTF |
| Print/Design | TTF or OTF | - |
| Email | TTF | - |
| Fallback | TTF | - |

## License Files

Each font directory contains a `LICENSE` file with complete license information:

```
fonts/vazir/LICENSE       - Vazir font license
fonts/roboto/LICENSE      - Roboto font license
fonts/ubuntu/LICENSE      - Ubuntu font license
fonts/inter/LICENSE       - Inter font license
fonts/lato/LICENSE        - Lato font license
fonts/opensans/LICENSE    - Open Sans font license
```

Always include these licenses when distributing fonts.

## README Files

Each font directory includes a `README.md` with:

- Font description
- Weight and style options
- Creator/designer information
- Installation instructions
- Usage examples
- License summary

Example structure:
```
fonts/vazir/README.md
fonts/roboto/README.md
fonts/ubuntu/README.md
```

## Variable Fonts

Some fonts include variable font versions:

- `FontName-Variable.ttf` - Variable font with all weights
- `FontName-Variable.woff2` - Variable font in WOFF2 format

Variable fonts reduce file size when multiple weights are needed.

## Usage Examples

### Example 1: Loading Single Weight

```css
@font-face {
  font-family: 'Roboto';
  src: url('/fonts/roboto/Roboto-Regular.woff2') format('woff2');
}

body {
  font-family: 'Roboto', sans-serif;
}
```

### Example 2: Loading Multiple Weights

```css
@font-face {
  font-family: 'Lato';
  font-weight: 300;
  src: url('/fonts/lato/Lato-Light.woff2') format('woff2');
}

@font-face {
  font-family: 'Lato';
  font-weight: 400;
  src: url('/fonts/lato/Lato-Regular.woff2') format('woff2');
}

@font-face {
  font-family: 'Lato';
  font-weight: 700;
  src: url('/fonts/lato/Lato-Bold.woff2') format('woff2');
}

body {
  font-family: 'Lato', sans-serif;
}

strong {
  font-weight: 700;
}
```

### Example 3: Self-Hosting with Preload

```html
<!-- Preload critical font -->
<link rel="preload" href="/fonts/vazir/Vazir.woff2" as="font" type="font/woff2" crossorigin>

<style>
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
</style>
```

## File Sizes

Typical file sizes (approximate):

| Font | Format | Size |
|------|--------|------|
| Vazir Regular | WOFF2 | ~45 KB |
| Roboto Regular | WOFF2 | ~65 KB |
| Ubuntu Regular | WOFF2 | ~55 KB |
| Inter Regular | WOFF2 | ~50 KB |
| Lato Regular | WOFF2 | ~48 KB |
| Open Sans Regular | WOFF2 | ~60 KB |

*Note: File sizes may vary based on character set and optimization*

## Performance Optimization Tips

1. **Use WOFF2** - Most compressed format
2. **Subsetting** - Include only needed characters
3. **Preloading** - Use `rel="preload"` for critical fonts
4. **Font Display** - Use `font-display: swap` to prevent blocking
5. **Variable Fonts** - Use variable fonts to reduce file count
6. **Lazy Load** - Load non-critical fonts after page load

## Troubleshooting

### Font Not Loading

- Check file path is correct
- Verify MIME types are set correctly on your server
- Use `crossorigin` attribute for cross-origin requests
- Check browser console for errors

### MIME Type Configuration

Configure your server to serve fonts with correct MIME types:

```apache
# .htaccess (Apache)
AddType application/font-woff2 .woff2
AddType application/font-woff .woff
AddType application/octet-stream .ttf
```

### Cross-Origin Issues

Include `crossorigin` attribute:

```html
<link rel="preload" href="/fonts/vazir/Vazir.woff2" as="font" type="font/woff2" crossorigin>
```

## Support & Questions

For issues or questions about accessing fonts:

1. Check this document
2. See individual font README files
3. Open an issue on GitHub
4. Check the main README.md

---

**Last Updated:** 2026-09-01
