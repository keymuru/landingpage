# Coach Snehal — Manifestation Landing Page

Three colour-theme variants of the landing page. Open each in a browser, pick the one you love, and follow the steps below.

---

## 📁 Files

| File | Theme |
|---|---|
| `theme-calm.html` | 🌸 Calm & Sacred — Soft Purple + Gold + Cream |
| `theme-bold.html` | 💼 Bold & Driven — Deep Navy + Orange + White |
| `theme-earthy.html` | 🌿 Earthy & Grounded — Forest Green + Terracotta + Beige |

---

## ✏️ Things to Replace Before Going Live

Open your chosen HTML file in any text editor (VS Code recommended) and search (`Ctrl+F` / `Cmd+F`) for each placeholder below.

### 1. Razorpay Payment Link
Search for: `YOUR_RAZORPAY_LINK_HERE`
Replace with your Razorpay payment page URL.

> **Important:** In your Razorpay dashboard, set the **Success Redirect URL** to your WhatsApp link (see below) so users land on WhatsApp automatically after payment.

### 2. WhatsApp Scheduling Link
After a user pays, they should land on WhatsApp to schedule. Set this as the Razorpay redirect URL:

```
https://wa.me/91XXXXXXXXXX?text=Hi%20Snehal!%20I%20just%20booked%20my%20discovery%20session%20and%20would%20love%20to%20schedule%20my%20time.
```
Replace `91XXXXXXXXXX` with Snehal's WhatsApp number (with country code, no `+`).

### 3. Instagram Link
Search for: `YOUR_INSTAGRAM_URL_HERE`
Replace with: `https://www.instagram.com/YOUR_HANDLE`

### 4. YouTube Link
Search for: `YOUR_YOUTUBE_URL_HERE`
Replace with: `https://www.youtube.com/@YOUR_CHANNEL`

### 5. Coach Bio (Optional)
Search for the `about-content` section and update Snehal's bio with her real story, credentials, and experience.

### 6. Countdown Duration (Optional)
Default is **48 hours** per visitor. To change it, find this line in the `<script>` section:
```js
var HOURS = 48;
```
Change `48` to whatever number of hours you want.

---

## 🚀 How to Host for Free

### Option A — Netlify (Easiest, Recommended)
1. Go to [netlify.com](https://netlify.com) and create a free account.
2. Click **"Add new site" → "Deploy manually"**.
3. Drag and drop your chosen HTML file into the upload area.
4. Done — Netlify gives you a free `your-site.netlify.app` URL instantly.
5. (Optional) Connect a custom domain you own.

### Option B — GitHub Pages (Free)
1. Create a free [GitHub](https://github.com) account.
2. Create a new repository (e.g. `coach-snehal-landing`).
3. Upload your chosen HTML file and **rename it to `index.html`**.
4. Go to **Settings → Pages → Source: main branch** and save.
5. Your site will be live at `https://USERNAME.github.io/coach-snehal-landing`.

### Option C — Vercel (Free)
1. Go to [vercel.com](https://vercel.com) and sign in with GitHub.
2. Import your GitHub repository.
3. Vercel auto-detects the HTML file and deploys it.

---

## 🛠 Customisation Tips

- **Logo / Name** — Search for `Coach Snehal` in the HTML to update the name everywhere.
- **Spots count** — The number of "spots left" is stored per visitor in their browser. Change the range in the JS section: `Math.floor(Math.random() * 4) + 7` gives 7–10.
- **Session language** — The page currently says "Hindi & English". Update if language preferences change.
- **Testimonials** — Replace the placeholder testimonials with real ones for higher trust.
- **Illustration** — The coach illustration is SVG — it's fully scalable and loads fast. Replace with a real photo by swapping the `<svg>` tag with an `<img>` tag pointing to your image file.

---

## 📱 Mobile & Desktop

All three pages are fully responsive:
- **Mobile (<640px)** — Single column, large tap targets, floating sticky Book button
- **Tablet (640–1024px)** — 2–3 column grids where appropriate
- **Desktop (>1024px)** — Wide layout with illustration beside hero text, 3-col grids

---

## 📊 Tracking (Future)

When you're ready to add a Facebook Pixel for Instagram ad conversion tracking:
1. Get your Pixel ID from Meta Business Suite.
2. Paste the Meta Pixel base code just before `</head>` in your HTML.
3. Add a `Purchase` event after the payment redirect if Razorpay supports it.

---

*Built for Coach Snehal · © 2026*
