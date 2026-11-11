# Rafter & Rose — romantic cottage garden website

## What is included
- `index.html` — Home
- `menu.html` — Menu
- `events.html` — Events
- `private-hire.html` — Private Hire
- `cakes.html` — Cake Orders
- `contact.html` — Contact
- `assets/style.css` — site styling
- `assets/script.js` — mobile menu and email enquiry forms

## IMPORTANT before launch
1. **Enquiry forms are not operational yet.** In `assets/script.js`, replace `YOUR_EMAIL@example.com` with the real café enquiries email. Forms use the visitor's own email application (mailto), not a backend; they cannot guarantee submission. For a reliable form, later use a hosted form service or Supabase.
2. Replace stock illustrative photos with photos you own or have permission to use. Images currently load from Unsplash remotely; they require an internet connection.
3. Replace menu placeholders with real menu items/prices, confirmed events/tickets, actual venue details, cake details, and street address.
4. Confirm café hours, event/hire terms, and copy.
5. Rewards links go to https://rewards.rafterandrose.com/ but **the Rewards app remains a prototype**. Do not advertise real reward earning or redemption until the backend and security controls are built.
6. Google Fonts are remotely loaded; website will fall back to system fonts without internet.

## Publish for free using GitHub Pages (separate from Rewards)
1. In GitHub, create a NEW public repository, e.g. `rafter-rose-website`. Do not modify the existing Rewards repository.
2. Unzip the download and upload all six `.html` files and the `assets` folder to the root of the new repository. (GitHub web upload can accept the files/folder; ensure paths are preserved.)
3. Go to repository Settings → Pages → Deploy from a branch → `main` → `/(root)` → Save.
4. Test the initial URL `https://vt2vgw2d76-alt.github.io/rafter-rose-website/` (assuming that repository name).
5. **Only after testing** configure `rafterandrose.com` as the custom domain in this NEW repository's Settings → Pages. GitHub Pages will then instruct you to configure Squarespace DNS for the apex domain. The four GitHub Pages A records are `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`; optionally configure `www` CNAME to `vt2vgw2d76-alt.github.io`. Do not remove MX/TXT records for email or the `rewards` CNAME. Verify current GitHub documentation before changing DNS.
6. After DNS validation, enable Enforce HTTPS when available.

## Design notes
This is a static, responsive, multi-page website with a romantic cottage-garden look. No CMS or backend is included; menu/event edits require editing the HTML files.
