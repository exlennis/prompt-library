- Inspect Website
- Broswer, 
- Claude 3.5, 1/5 Low Temp 

## Promopt
```markdown
Describe me the tech stack used based on the following HTML document:

{browser-tab format="html"}

Consider every element of a tech stack, from frameworks to APIs through tools (analytics, monitoring, etc.). Include which fonts are used. Don't make any guesses on what’s used if there’s no evidence.
```

---

## Example Input & Ouput


### Example 1
**User Input:** https://p.cv

**LLM Output:**
```markdown
Based on the HTML document, here's the observed tech stack for p.cv:

### Frontend
- **HTML5**
  - Uses modern HTML5 semantic structure
  - Responsive design with mobile/desktop variants
  - Uses `data-theme` attribute for theme switching

- **CSS**
  - Custom CSS file: `pcv.css`
  - CSS variables for theming
  - Responsive design with mobile-specific classes

- **JavaScript**
  - Vanilla JavaScript (no framework detected)
  - Uses ES6+ features like `const`, arrow functions
  - Modular JavaScript with ES6 module imports (`type="module"`)

### External Services & APIs
- **Google Analytics**
  - Google Tag Manager script
  - Tracking ID: G-77VL7HJBW8

### Tools & Utilities
- **Clipboard API** (for email copying)
- **Local Storage** (for theme persistence)
- **Prefers Color Scheme** media query (for default theme detection)

### Asset Management
- **Favicon**: `favicon.png`
- **Apple Touch Icon**: `icon.png`
- **Open Graph Images**: `pcv.png`

### Modules
- Custom modules:
  - `/src/run.js`
  - `/ascii.js`

### Fonts
- No specific font information is evident in the HTML

### Hosting/Deployment
- No specific hosting information is visible

### Browser Compatibility
- Uses `X-UA-Compatible` meta tag for IE compatibility
- Responsive viewport meta tag

### Interactivity Features
- Theme toggling
- External link opening
- Email interaction (copy/mailto)
```

### Example 3
**User Input:** https://studioblackburn.com

**LLM Output:**
```markdown
Based on the HTML document, here's the identified tech stack for Studio Blackburn's website:

## Frontend
- **Framework/Library**: Not definitively identified
- **JavaScript**: 
  - Custom JavaScript (bundle.js)
  - Matomo tracking script

## Styling
- **CSS**: 
  - Custom CSS (bundle.css)
  - Inline styles

## Fonts
- **Web Fonts**: 
  - Hosted on Radim Pesko's webfont service (webfonts2.radimpesko.com)

## Analytics & Tracking
- **Web Analytics**: 
  - Matomo (self-hosted analytics platform)
  - Tracking URL: https://stats.theworkers.net/matomo.js

## Performance & Optimization
- **Lazy Loading**: Evidence of image lazy loading and dynamic content loading
- **Responsive Design**: Viewport meta tag for responsive rendering

## External Services
- **Form Handling**: 
  - Jobs application form via Tally (https://tally.so/r/wgqGPP)

## Social & Communication
- **Social Media Links**:
  - Instagram
  - LinkedIn

## Additional Observations
- Uses semantic HTML5 structure
- Implements Open Graph metadata for social sharing
- Supports no-JavaScript fallback
```

