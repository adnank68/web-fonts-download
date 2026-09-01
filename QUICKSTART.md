# Quick Start Guide

Welcome to Web Fonts Download! This guide will help you quickly get started with the Vazir and Roboto fonts.

## 🚀 Quick Links

### Vazir Font (Persian)
- **Download Guide:** [fonts/vazir/DOWNLOAD.md](./fonts/vazir/DOWNLOAD.md)
- **Font Documentation:** [fonts/vazir/README.md](./fonts/vazir/README.md)
- **License:** [fonts/vazir/LICENSE](./fonts/vazir/LICENSE) (SIL OFL)
- **Official Repository:** https://github.com/rastikerdar/vazir-font

### Roboto Font (English)
- **Download Guide:** [fonts/roboto/DOWNLOAD.md](./fonts/roboto/DOWNLOAD.md)
- **Font Documentation:** [fonts/roboto/README.md](./fonts/roboto/README.md)
- **License:** [fonts/roboto/LICENSE](./fonts/roboto/LICENSE) (Apache 2.0)
- **Official Repository:** https://github.com/google/fonts/tree/main/apache/roboto
- **Google Fonts:** https://fonts.google.com/specimen/Roboto

---

## 📥 Downloading Fonts

### Method 1: Download from Official Sources (Recommended)

#### For Vazir:
1. Visit: https://github.com/rastikerdar/vazir-font/releases/latest
2. Download the ZIP file containing all formats
3. Extract and use the WOFF2 files for web

#### For Roboto:
1. Visit: https://fonts.google.com/specimen/Roboto
2. Click "Download family"
3. Use the WOFF2 files for web

### Method 2: Direct Download Links

**Vazir Font:**
- TTF: https://github.com/rastikerdar/vazir-font/blob/master/dist/Vazir-Regular.ttf?raw=true
- WOFF2: https://github.com/rastikerdar/vazir-font/blob/master/dist/Vazir-Regular.woff2?raw=true
- Bold: https://github.com/rastikerdar/vazir-font/blob/master/dist/Vazir-Bold.woff2?raw=true

**Roboto Font:**
- TTF: https://github.com/google/fonts/blob/main/apache/roboto/Roboto-Regular.ttf?raw=true
- WOFF2: https://fonts.gstatic.com/s/roboto/v30/KFOmCnqEu92Fr1Mu4mxP.woff2
- Bold: https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmWUlfCRc_.woff2

---

## 🎨 Using Fonts in Your Website

### Step 1: Download Fonts
Choose your preferred method above and download the WOFF2 files.

### Step 2: Copy to Your Server
```
your-website/
├── css/
│   └── style.css
├── fonts/
│   ├── vazir/
│   │   ├── Vazir.woff2
│   │   └── Vazir-Bold.woff2
│   └── roboto/
│       ├── Roboto-Regular.woff2
│       └── Roboto-Bold.woff2
```

### Step 3: Add CSS

```css
/* Load fonts */
@font-face {
  font-family: 'Vazir';
  src: url('/fonts/vazir/Vazir.woff2') format('woff2');
  font-weight: normal;
  font-display: swap;
}

@font-face {
  font-family: 'Vazir';
  src: url('/fonts/vazir/Vazir-Bold.woff2') format('woff2');
  font-weight: bold;
  font-display: swap;
}

@font-face {
  font-family: 'Roboto';
  src: url('/fonts/roboto/Roboto-Regular.woff2') format('woff2');
  font-weight: normal;
  font-display: swap;
}

@font-face {
  font-family: 'Roboto';
  src: url('/fonts/roboto/Roboto-Bold.woff2') format('woff2');
  font-weight: bold;
  font-display: swap;
}

/* Use fonts */
body {
  font-family: 'Roboto', sans-serif;
}

/* For Persian text */
.persian {
  font-family: 'Vazir', sans-serif;
  direction: rtl;
}
```

### Step 4: Use in HTML

```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <link rel="stylesheet" href="css/style.css">
</head>
<body>
  <h1>Welcome to Web Fonts</h1>
  <p>This text uses Roboto font.</p>
  <p class="persian">این متن از فونت وزیر استفاده می‌کند</p>
</body>
</html>
```

---

## ⚡ Performance Tips

1. **Use WOFF2 Format**
   - Smallest file size
   - Excellent browser support
   - Recommended for web use

2. **Preload Critical Fonts**
   ```html
   <link rel="preload" href="/fonts/roboto/Roboto-Regular.woff2" as="font" type="font/woff2" crossorigin>
   ```

3. **Use font-display: swap**
   - Shows fallback text immediately
   - Prevents invisible text
   - Better user experience

4. **Only Load Weights You Use**
   - Don't load all weights
   - Load only Regular (400) and Bold (700) if that's all you need
   - Reduces bandwidth

5. **Self-Host Fonts**
   - Faster than CDN in many cases
   - Better privacy for users
   - Full control over fonts

---

## ✅ Legal Information

### ✅ You CAN:
- Use for commercial projects
- Use on websites
- Use in applications
- Modify fonts
- Redistribute (with attribution)

### ❌ You CANNOT:
- Sell fonts alone
- Remove attribution
- Claim ownership
- Redistribute without license

**Full Legal Details:** See [LEGAL.md](./LEGAL.md)

---

## 📚 Documentation Files

| File | Purpose |
|------|---------|
| [README.md](./README.md) | Main documentation |
| [LEGAL.md](./LEGAL.md) | Legal information |
| [CREDITS.md](./CREDITS.md) | Font creator credits |
| [CONTRIBUTING.md](./CONTRIBUTING.md) | How to contribute |
| [FONTS-DIRECTORY.md](./FONTS-DIRECTORY.md) | Font directory structure |
| [package.json](./package.json) | Project metadata |

---

## 🎯 Font Comparison

| Feature | Vazir | Roboto |
|---------|-------|--------|
| Language | Persian/Arabic | English/Latin |
| Creator | Saber Rastikerdar | Google |
| License | SIL OFL | Apache 2.0 |
| Weights | Regular, Bold | 5+ weights |
| Best For | Persian text | General web/UI |
| File Size | ~45-48 KB (WOFF2) | ~50-65 KB (WOFF2) |

---

## 🔗 Resources

- **Vazir Font:** https://github.com/rastikerdar/vazir-font
- **Roboto Font:** https://fonts.google.com/specimen/Roboto
- **SIL OFL License:** https://scripts.sil.org/OFL
- **Apache 2.0 License:** https://www.apache.org/licenses/LICENSE-2.0
- **MDN @font-face:** https://developer.mozilla.org/en-US/docs/Web/CSS/@font-face
- **Web Font Best Practices:** https://web.dev/font-best-practices/

---

## ❓ FAQ

**Q: Can I use these fonts commercially?**
A: Yes! Both Vazir and Roboto are free for commercial use.

**Q: Do I need to credit the creators?**
A: Yes, always include the LICENSE file with distributions and credit the creators.

**Q: Which format should I use for web?**
A: Use WOFF2. It's the smallest and has excellent browser support.

**Q: Can I modify the fonts?**
A: Yes, but you must rename them and include the license.

**Q: Can I sell products using these fonts?**
A: Yes! You can sell software/services using these fonts. You cannot sell the fonts themselves.

---

## 🚀 Next Steps

1. **Download Fonts**
   - See download guides in each font directory

2. **Copy to Your Server**
   - Create a `/fonts/` directory on your web server

3. **Add CSS**
   - Include @font-face rules in your stylesheet

4. **Use in HTML**
   - Apply fonts to your HTML elements

5. **Test and Deploy**
   - Verify fonts load correctly
   - Deploy to production

---

## 📞 Support

- **Vazir Support:** https://github.com/rastikerdar/vazir-font/issues
- **Roboto Support:** https://github.com/google/fonts/issues
- **This Repository:** https://github.com/adnank68/web-fonts-download

---

**Happy font usage! 🎨**

**Last Updated:** 2026-09-01
