# Caveman Converter

> Transform your sophisticated modern English into authentic prehistoric cave-speak. 🦴

## What It Does

The Caveman Converter uses an AI language model (Groq's llama-3.1-8b-instant) to intelligently rewrite modern English as authentic caveman speech. It drops articles, simplifies verbs, and maintains meaning while producing short, grunting, brutalist language.

**Input:** "The ancient civilizations have developed sophisticated technologies and remarkably advanced architectural structures."  
**Output:** "Old tribe build strong things Old tribe make sharp rock tools, build big houses. Rock houses stand long time."

Supports plain text (`.txt`) and Markdown (`.md`) files with structure preservation. 100% client-side — no server required.

## How to Use

### Online (Easiest)
1. Go to [caveman-converter GitHub Pages](https://kishore3656.github.io/caveman-converter/) (if deployed)
2. Or: Go to [app.netlify.com/drop](https://app.netlify.com/drop)
3. Drag the `index.html` file into the browser window
4. Get a live public URL instantly — no signup required
5. **Important:** The app needs a valid Groq API key (stored in `.env`) to work

### Local (Quick Start)
1. Clone this repository: `git clone https://github.com/Kishore3656/caveman-converter.git`
2. Create a `.env` file with your Groq API key:
   ```
   GROQ_API_KEY=gsk_your_key_here
   ```
3. Open `index.html` in any modern web browser (Chrome, Firefox, Safari, Edge)
4. Start converting!

**Getting a Free Groq API Key:**
1. Go to [console.groq.com](https://console.groq.com)
2. Sign up (free, no credit card required)
3. Create an API key
4. Paste it into your `.env` file

### Features
- **Type It Mode:** Paste or type modern English directly into the left panel
- **File Upload Mode:** Drag & drop `.txt` or `.md` files to convert entire documents
- **Markdown Support:** Preserves headings, lists, blockquotes, and code blocks while converting text
- **One-Click Download:** Save converted output with a single click
- **100% Client-Side:** No server, no internet required after loading — all processing happens in your browser

## How It Works

The converter uses **Groq's llama-3.1-8b-instant** model to intelligently rewrite text. The AI understands:

1. **Articles & Helpers:** Drops "the", "a", "an", "is", "are", "was", etc.
2. **Verb Simplification:** Converts past tense to simple forms (went → go, bought → buy)
3. **Adjective/Adverb Reduction:** Simplifies descriptors (quickly → quick, amazing → amazing things)
4. **Repetition:** Caveman speech is repetitive and grunting
5. **Meaning Preservation:** Always keeps the core message understandable

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
| AI Model | [Groq](https://groq.com) llama-3.1-8b-instant | $0 (free tier) |
| Hosting | Netlify Drop or GitHub Pages (free tier) | $0 |
| **Total** | | **$0** |

**Free Tier Details:**
- Groq free tier: 14,400 requests/day, 30 requests/min, no credit card required
- Perfect for a public demo site — the free quota is plenty for typical usage

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
