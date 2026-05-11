# Caveman Converter

> Transform your sophisticated modern English into authentic prehistoric cave-speak. 🦴

## What It Does

The Caveman Converter strips stop words, removes morphological suffixes (`-ing`, `-ed`, `-ly`), and applies irregular verb mapping to produce terse, brutalist caveman language. 

**Input:** "I went to the store and bought some amazing things."  
**Output:** "Go store bought things."

Supports plain text (`.txt`) and Markdown (`.md`) files with structure preservation.

## How to Use

### Online (No Installation)
1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag the `index.html` file into the browser window
3. Get a live public URL instantly — no signup required

### Local (Quick Start)
1. Save the `index.html` file to your computer
2. Open it in any modern web browser (Chrome, Firefox, Safari, Edge)
3. Start converting

### Features
- **Type It Mode:** Paste or type modern English directly into the left panel
- **File Upload Mode:** Drag & drop `.txt` or `.md` files to convert entire documents
- **Markdown Support:** Preserves headings, lists, blockquotes, and code blocks while converting text
- **One-Click Download:** Save converted output with a single click
- **100% Client-Side:** No server, no internet required after loading — all processing happens in your browser

## Conversion Rules

The converter applies these transformations in order:

1. **Stop Words Removed:** the, a, an, is, are, was, were, be, have, has, do, does, very, really, just, etc.
2. **Suffix Stripping:**
   - `-ing` → stripped (running → run)
   - `-ed` → stripped (walked → walk)
   - `-ly` → stripped (quickly → quick)
3. **Irregular Verb Mapping:** went → go, ran → run, came → come, made → make, etc.
4. **Whitespace Collapsed:** Multiple spaces reduced to one

**Protected Content:**
- Code blocks (fenced with ``` or indented with 4 spaces)
- Markdown syntax (# headings, > quotes, - lists remain intact)

## Examples

### Plain Text
```
Input:  "The ancient civilizations created remarkable monuments."
Output: "Ancient civilizations created remarkable monuments."
```

### Markdown
```markdown
Input:
# The Modern World
We have advanced technology and sophisticated systems.

Output:
# Modern World
Advanced technology systems.
```

## Hosting (Free, Forever)

### Option 1: Netlify (Easiest)
1. Visit [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag `index.html` into the window
3. Get a live URL — done! (~5 seconds)
4. (Optional) Sign up to keep the URL permanent and rename it

### Option 2: GitHub Pages
1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch
4. Live at `https://yourusername.github.io/caveman-converter`

### Option 3: Local File
- Just open `index.html` in your browser directly (no web server needed)

## Tech Stack

| Component | Technology | Cost |
|---|---|---|
| Framework | Pure HTML5 / CSS3 / Vanilla JS | $0 |
| Display Fonts | [Uncial Antiqua](https://fonts.google.com/specimen/Uncial+Antiqua) (Google Fonts) | $0 |
| Markdown Parsing | [marked.js v12](https://marked.js.org/) (CDN) | $0 |
| Hosting | Netlify Drop (free tier) | $0 |
| **Total** | | **$0** |

## Browser Support

- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+
- Any browser with ES6 JavaScript support

## Development

The entire app is a single `index.html` file with no build process:

```bash
# Test locally
open index.html

# Or from terminal
npx http-server

# Push to GitHub
git add .
git commit -m "Caveman converter live"
git push origin main
```

No `npm install`, no build step, no framework overhead.

## Features

✅ Type or paste English text  
✅ Upload `.txt` or `.md` files  
✅ Real-time preview  
✅ One-click download  
✅ Markdown structure preservation  
✅ 100% client-side (zero latency)  
✅ Responsive design  
✅ No account required  
✅ No tracking, no ads, no nonsense  

## Error Handling

| Trigger | Output |
|---|---|
| Empty input on translate | `Ug. No words. Cave empty.` |
| Empty file uploaded | `File empty. Ug.` |
| Wrong file type (.doc, .pdf, etc.) | `Cave no understand. Use .txt or .md only.` |
| Save with no output | `Ug. No words. Cave empty.` (appears in output area) |

## Keyboard Shortcuts

| Key | Action |
|---|---|
| **Type It / File Upload Toggle** | Click the pill switch or use your mouse |
| **Translate** | Click the **UNGA TRANSLATE** button |
| **Save** | Click the **SAVE** button |
| **Clear** | Click the **CLEAR** button |

## Privacy & Security

- ✅ 100% client-side — no server sees your text
- ✅ No cookies, no tracking, no analytics
- ✅ No internet connection required after loading
- ✅ All conversion happens in your browser only
- ✅ No data is stored, logged, or transmitted

## License

```
10,000 BC — Ug's Public License
Free to use, modify, share. No restrictions.
Ug no care about licensing.
```

## Feedback

- Report bugs: [GitHub Issues](https://github.com/Kishore3656/caveman-converter/issues)
- Suggest features: Open an issue with "enhancement" label
- Fork & improve: Pull requests welcome

---

**Made with ❤️ (and some fire) by the Modern Primitive Labs**

Go forth. Simplify your language. Become one with the cave.
