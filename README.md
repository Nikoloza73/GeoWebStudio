# GeoWebStudio — Website

A clean, modern, futuristic website for **GeoWebStudio** — a web design studio based in Tbilisi, Georgia.

---

## 🚀 How to Run

### Option 1 — VS Code Live Server (Recommended)
1. Open the `GeoWebStudio/` folder in VS Code
2. Install the **Live Server** extension (by Ritwick Dey) if you haven't
3. Right-click `index.html` → **Open with Live Server**
4. Your browser opens automatically at `http://127.0.0.1:5500`

### Option 2 — Open directly in browser
Simply double-click `index.html` — no server needed.
> Note: Google Fonts requires an internet connection to load correctly.

### Option 3 — GitHub Pages (Free Hosting)
1. Push this folder to a GitHub repository
2. Go to **Settings → Pages**
3. Set source to **main branch / root**
4. Your site is live at `https://yourusername.github.io/repo-name`

---

## 📁 Project Structure

```
GeoWebStudio/
├── index.html          # Main HTML file
├── css/
│   └── style.css       # All styles (variables, components, responsive)
├── js/
│   └── main.js         # Interactions, animations, form handling
└── README.md           # This file
```

---

## ✨ Features

- **Fully responsive** — looks great on mobile, tablet, and desktop
- **Custom cursor** with hover states (desktop only)
- **Scroll reveal animations** using IntersectionObserver
- **Animated stat counters** in the hero section
- **Smooth scrolling** to all sections
- **Active nav link** highlighting on scroll
- **Parallax** effect on hero background orbs
- **Mobile hamburger menu** with full-screen overlay
- **Contact form** with basic validation and success state
- **No dependencies** — pure HTML, CSS, JavaScript

---

## 🎨 Color Palette

| Name         | Value       |
|--------------|-------------|
| Navy 950     | `#03070f`   |
| Navy 900     | `#060e1e`   |
| Navy 800     | `#0a1628`   |
| Cyan 500     | `#00c8e0`   |
| Cyan 400     | `#22ddf5`   |
| Cyan 300     | `#6ef0ff`   |

---

## 🖋️ Fonts

- **Syne** — Display / headings (bold, futuristic)
- **DM Sans** — Body text (clean, readable)

Both loaded from Google Fonts.

---

## 📬 Connecting the Contact Form

The form currently simulates a submission. To make it real:

### Option A — Formspree (Free, easiest)
1. Sign up at [formspree.io](https://formspree.io)
2. Create a form and copy your endpoint
3. In `js/main.js`, replace the simulated submit with:
```js
const res = await fetch('https://formspree.io/f/YOUR_ID', {
  method: 'POST',
  headers: { 'Content-Type': 'application/json' },
  body: JSON.stringify({
    name: form.name.value,
    email: form.email.value,
    message: form.message.value,
  })
});
```

### Option B — EmailJS (Client-side, no backend)
See: [emailjs.com](https://www.emailjs.com)

---

## 🌐 Deployment Options

| Platform       | Cost  | Notes                              |
|----------------|-------|------------------------------------|
| GitHub Pages   | Free  | Easiest for static sites           |
| Netlify        | Free  | Drag-and-drop deploy               |
| Vercel         | Free  | Instant deploy from GitHub         |
| Your own host  | Paid  | Full control via FTP/cPanel        |

---

## 📝 Customization Checklist

- [ ] Replace placeholder email `hello@geowebstudio.ge` with your real email
- [ ] Update Telegram handle `@geowebstudio`
- [ ] Add your real project screenshots to the portfolio section
- [ ] Replace avatar initials `G` and `N` with your names
- [ ] Connect the contact form (Formspree recommended)
- [ ] Add your social media links in the footer
- [ ] Update meta description in `<head>` for SEO
- [ ] Add a `favicon.ico` to the root folder

---

Built with ❤️ in Georgia 🇬🇪
