# Your Business Website

A fast, modern, responsive static website for your business. Built with plain HTML/CSS/JS for easy hosting anywhere.

## Structure

- `index.html` – Home
- `about.html` – About page
- `services.html` – Services page
- `contact.html` – Contact with form and details
- `css/style.css` – Global styles and theme
- `js/main.js` – Small enhancements (year, mobile nav)
- `assets/logo.svg`, `assets/favicon.svg` – Branding

## Customize

1. Replace the name "Your Business" in all pages with your business name.
2. Update text content on each page (hero, features, services, contact details).
3. Update `assets/logo.svg` with your logo (or replace the file).
4. Update contact details in `contact.html` (email, phone, hours).
5. Optional: Replace `assets/favicon.svg` with your custom favicon.

## Contact Form Options

- Quick: Set `action` in `contact.html` form to a Formspree or Getform endpoint.
- Mailto: Remove the form `action` and use the Email button (`mailto:` link).
- Self-hosted: Connect to your backend POST endpoint and handle CORS.

## Run Locally

Open `index.html` directly in your browser, or serve the folder:

```bash
# Python 3
python -m http.server 5173

# Node (if installed)
npx serve . -l 5173 --single
```

Then visit `http://localhost:5173`.

## Deploy Online (Free Options)

### Option 1: Netlify (Easiest - No coding needed)
1. Go to https://www.netlify.com and sign up (free)
2. Drag and drop your entire `local` folder onto the Netlify dashboard
3. Your site is live! You'll get a URL like `your-site-name.netlify.app`
4. **Note:** Your orders are stored in browser localStorage, so they won't sync across devices. For production, consider a backend.

### Option 2: GitHub Pages (Free, Good for updates)
1. Create account at https://github.com
2. Create a new repository (e.g., "sakthi-mobiles-pos")
3. Upload all files from your `local` folder to the repository
4. Go to Settings → Pages → Select `main` branch → Save
5. Your site will be at `your-username.github.io/repository-name`

### Option 3: Vercel (Free, Fast)
1. Go to https://vercel.com and sign up
2. Click "Add New Project" → Import your folder
3. Deploy - site goes live immediately

### Important Notes for Deployment:
- **localStorage data**: Orders are saved in the browser, not on a server. Each device/browser has its own data.
- **QR Code**: Make sure to upload your GPay QR image before deploying, or users can upload it after.
- **HTTPS**: All these platforms provide free HTTPS (secure connection).

## Notes

- No build step. Pure static files.
- Performance-friendly styles; accessible colors and contrasts.
- Mobile nav toggles via the ☰ button.



