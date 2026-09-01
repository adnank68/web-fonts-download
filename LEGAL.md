# Legal Information

## Disclaimer

All fonts included in this repository are open-source and provided under permissive licenses that allow free use, modification, and distribution. This document outlines the legal framework for using these fonts.

## Font Licenses Overview

### What is Permitted

✅ **Use on Websites** - Embed and display fonts on any website  
✅ **Commercial Use** - Use in commercial projects without licensing fees  
✅ **Self-Hosting** - Host fonts on your own servers  
✅ **Modification** - Modify fonts (subset, optimize, etc.)  
✅ **Redistribution** - Share fonts with others  
✅ **Desktop Applications** - Use in desktop software  
✅ **Mobile Applications** - Use in mobile apps  
✅ **Print Materials** - Use for printed designs  

### What is NOT Permitted

❌ **Selling Fonts Alone** - Don't sell the font files as a commercial product  
❌ **Removing Attribution** - Don't remove creator credit or license files  
❌ **Trademark Misuse** - Don't claim to own the font or misrepresent its origin  
❌ **Removing License Terms** - Don't distribute without including the license  

## Font-Specific Legal Information

### Vazir Font (SIL OFL)

**License:** SIL Open Font License v1.1  
**Creator:** Saber Rastikerdar  

**You can:**
- Use freely on websites and applications
- Modify and create derivatives
- Distribute modified versions (with attribution)
- Use commercially

**You must:**
- Include the OFL license text
- Credit Saber Rastikerdar
- Not claim ownership of the original font

**Reference:** See `fonts/vazir/LICENSE` for full license text

---

### Roboto Font (Apache 2.0)

**License:** Apache License 2.0  
**Creator:** Google Inc.  

**You can:**
- Use freely on websites and applications
- Modify and create derivatives
- Distribute modified versions (with attribution)
- Use commercially

**You must:**
- Include the Apache 2.0 license text
- Include a NOTICE file with attribution
- State significant changes made

**Reference:** See `fonts/roboto/LICENSE` for full license text

---

### Ubuntu Font (Ubuntu Font License)

**License:** Ubuntu Font License v1.0  
**Creator:** Canonical Ltd., designed by Dalton Maag  

**You can:**
- Use freely on websites and applications
- Modify and create derivatives
- Distribute (with attribution)

**You must:**
- Include the Ubuntu Font License text
- Credit Canonical Ltd. and Dalton Maag
- Follow specific naming conventions for derivatives

**Reference:** See `fonts/ubuntu/LICENSE` for full license text

---

### Inter Font (SIL OFL)

**License:** SIL Open Font License v1.1  
**Creator:** Rasmus Andersson  

**You can:**
- Use freely on websites and applications
- Modify and create derivatives
- Distribute modified versions
- Use commercially

**You must:**
- Include the OFL license text
- Credit Rasmus Andersson
- Not claim ownership

**Reference:** See `fonts/inter/LICENSE` for full license text

---

### Lato Font (SIL OFL)

**License:** SIL Open Font License v1.1  
**Creator:** Łukasz Dziedzic  

**You can:**
- Use freely on websites and applications
- Modify and create derivatives
- Distribute modified versions
- Use commercially

**You must:**
- Include the OFL license text
- Credit Łukasz Dziedzic
- Not claim ownership

**Reference:** See `fonts/lato/LICENSE` for full license text

---

### Open Sans (Apache 2.0)

**License:** Apache License 2.0  
**Creator:** Google Inc., designed by Steve Matteson  

**You can:**
- Use freely on websites and applications
- Modify and create derivatives
- Distribute modified versions
- Use commercially

**You must:**
- Include the Apache 2.0 license text
- Include NOTICE with attribution
- Document changes made

**Reference:** See `fonts/opensans/LICENSE` for full license text

---

## Implementation Guide

### For Websites

When hosting fonts from this repository on your website, include a credits page:

```html
<footer>
  <p>This website uses open-source fonts:</p>
  <ul>
    <li>Vazir Font by Saber Rastikerdar (SIL OFL)</li>
    <li>Roboto Font by Google (Apache 2.0)</li>
    <li>[Other fonts...]</li>
  </ul>
  <p>All fonts are open-source and distributed under their respective licenses.</p>
</footer>
```

### For Applications

Include license information in your application's About or Credits section:

```
OPEN SOURCE FONTS

This application includes the following open-source fonts:

1. Vazir Font
   Creator: Saber Rastikerdar
   License: SIL Open Font License v1.1
   URL: https://github.com/rastikerdar/vazir-font

2. Roboto Font
   Creator: Google Inc.
   License: Apache License 2.0
   URL: https://github.com/google/roboto

[Additional fonts...]

License texts are available in the application resources.
```

### For Distributed Software

Include the license files in your distribution:

```
MyApp/
├── resources/
│   ├── fonts/
│   │   ├── Vazir.ttf
│   │   ├── Vazir-LICENSE.txt
│   │   ├── Roboto.ttf
│   │   └── Roboto-LICENSE.txt
├── LICENSE
└── NOTICE.txt
```

---

## Common Scenarios

### Scenario 1: Using Fonts on a Commercial Website

**Question:** Can I use these fonts on my commercial website?  
**Answer:** ✅ **Yes.** All fonts in this repository permit commercial use. Simply include attribution and license files.

---

### Scenario 2: Modifying Fonts

**Question:** Can I modify the font files?  
**Answer:** ✅ **Yes.** You can modify fonts (subset for web, adjust weights, etc.). For OFL fonts, modified versions must be renamed and distributed with the OFL license. For Apache 2.0 fonts, document your changes.

---

### Scenario 3: Redistributing in a Package

**Question:** Can I include these fonts in my software package?  
**Answer:** ✅ **Yes.** Include the font files AND their license files in your package. Add attribution in your application's About/Credits section.

---

### Scenario 4: Selling a Product Using These Fonts

**Question:** Can I sell software that uses these fonts?  
**Answer:** ✅ **Yes.** You can sell software that uses these fonts (e.g., a design application, website theme). You cannot sell the fonts themselves as a standalone product. Include licenses and attribution.

---

### Scenario 5: Creating a Font Package

**Question:** Can I create a package that includes these fonts and sell it?  
**Answer:** ❌ **No.** You cannot sell fonts alone. However, you CAN bundle them with added value (e.g., design templates, usage guide, icon sets) while respecting the licenses.

---

## Warranty and Liability

**These fonts are provided "as is" without warranty.**

The creators and maintainers of these fonts provide them without any warranty, express or implied. Use at your own risk. Neither Saber Rastikerdar, Google Inc., Canonical Ltd., nor any other copyright holders shall be liable for any damage or loss arising from the use of these fonts.

---

## Attribution Examples

### Example 1: Website Footer
```html
<footer>
  <p>© 2026 My Website. Typography by Vazir (Saber Rastikerdar, SIL OFL)</p>
</footer>
```

### Example 2: Application Credits
```
Fonts Used:
• Vazir by Saber Rastikerdar - Persian typography
• Roboto by Google - Interface typography
Licensed under SIL OFL and Apache 2.0 respectively.
```

### Example 3: Design File
```
Fonts:
- Heading: Roboto Bold (Google, Apache 2.0)
- Body: Roboto Regular (Google, Apache 2.0)
- Persian Text: Vazir Regular (Saber Rastikerdar, SIL OFL)
All fonts are open-source and free for commercial use.
```

---

## Questions?

If you have questions about the legal use of these fonts:

1. **Review the specific font's license** in the `fonts/[fontname]/LICENSE` directory
2. **Check the font creator's repository** for additional documentation
3. **Consult the license text:** 
   - SIL OFL: https://scripts.sil.org/OFL
   - Apache 2.0: https://www.apache.org/licenses/LICENSE-2.0
   - Ubuntu Font: https://launchpad.net/ubuntu-font-family/+license

---

## Summary

**Bottom Line:** All fonts in this repository are free to use commercially on websites, in applications, and in print. Just include the license files and credit the creators. You cannot sell the fonts themselves, but you can sell products and services that use them.

---

**Last Updated:** 2026-09-01  
**Status:** Current and Accurate
