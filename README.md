# Social Media Downloader - Landing Page

A modern, responsive landing page for a social media video downloader service. Built with pure HTML, CSS, and vanilla JavaScript—no frameworks required.

## ✨ Features

- **Fully Responsive Design** – Works seamlessly on desktop, tablet, and mobile devices
- **Dark Mode Support** – Automatically adapts to system preferences using `prefers-color-scheme`
- **Smooth Scroll Animations** – Elements fade in as you scroll down the page
- **Sticky Navigation** – Header stays visible with blur backdrop effect
- **Mobile Menu** – Slide-down navigation drawer for smaller screens
- **6 Platform Cards** – Showcases support for YouTube, Instagram, TikTok, Facebook, X/Twitter, and Vimeo
- **Interactive FAQ Section** – Expandable details elements for common questions
- **Testimonials Grid** – User reviews with avatar placeholders
- **How It Works Section** – Step-by-step visual guide
- **Zero Dependencies** – No build tools, no npm packages, just pure web technologies

## 🎨 Design Highlights

- **Modern Aesthetic** – Glassmorphism effects, rounded corners, subtle shadows
- **Plus Jakarta Sans Font** – Clean, professional typography from Google Fonts
- **Remix Icon Library** – Beautiful icons via CDN
- **CSS Variables** – Easy theme customization for light/dark modes
- **Smooth Transitions** – Hover effects and animations throughout

## 📁 Project Structure

```
social-media-downloader/
├── index.html          # Main landing page (self-contained)
├── README.md           # This file
└── img/
    └── hero.png        # Hero section image (referenced in CSS)
```

## 🚀 Getting Started

### Option 1: Direct Usage
Simply open `index.html` in any modern web browser. No server required!

### Option 2: Local Development Server
For a better development experience with live reload:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (http-server)
npx http-server -p 8000

# Using PHP
php -S localhost:8000
```

Then visit `http://localhost:8000` in your browser.

## 🖼️ Adding the Hero Image

Place your hero image at `/img/hero.png` or update the CSS background URL on line 277:

```css
.hero-img {
    background: url("/img/hero.png") center/cover no-repeat;
}
```

Recommended image dimensions: **800×800px** (1:1 aspect ratio)

## 🎨 Customization

### Colors
All colors are defined as CSS variables in `:root`. Update these to match your brand:

```css
:root {
    --primary: #13c8ec;       /* Main brand color */
    --bg-light: #f6f8f8;      /* Light mode background */
    --bg-dark: #101f22;       /* Dark mode background */
    /* ... more variables ... */
}
```

### Typography
Change the font by replacing the Google Fonts import URL in the `<head>`:

```html
<link href="https://fonts.googleapis.com/css2?family=Your+Font:wght@400;700&display=swap" rel="stylesheet" />
```

Then update the `font-family` in the CSS.

### Content
All text content is easily editable directly in the HTML. Look for:
- Hero section headings and descriptions
- Platform cards (YouTube, Instagram, etc.)
- Features section benefits
- Testimonials
- FAQ items

## 📱 Responsive Breakpoints

- **Mobile:** `< 640px`
- **Tablet:** `640px - 864px`
- **Desktop:** `> 864px`

The layout automatically adjusts grid columns, padding, and navigation style based on screen size.

## 🎭 JavaScript Features

### Mobile Menu Toggle
```javascript
menuBtn.addEventListener("click", toggleMenu);
```
Opens/closes the mobile navigation drawer and swaps hamburger/close icons.

### Scroll Animations
```javascript
const observer = new IntersectionObserver(entries => { ... });
```
Uses the Intersection Observer API to fade in sections as they enter the viewport.

## 🌐 Browser Support

- ✅ Chrome/Edge (latest 2 versions)
- ✅ Firefox (latest 2 versions)
- ✅ Safari 14+
- ✅ iOS Safari 14+
- ✅ Android Chrome

**Note:** Dark mode requires browser support for `prefers-color-scheme` media query (all modern browsers).

## 📄 License

This is a demo landing page design. Feel free to use, modify, and distribute for personal or commercial projects.

## 🤝 Contributing

This is a standalone HTML file, but suggestions are welcome! To improve:

1. Test on different devices/browsers
2. Optimize images for faster loading
3. Add more accessibility features (ARIA labels)
4. Implement actual download functionality (backend required)

## 📞 Support

For questions or issues with the design:
- Email: support@dldr.com
- Phone: +1 (234) 567-890

---

**Built with ❤️ using HTML, CSS, and JavaScript**
