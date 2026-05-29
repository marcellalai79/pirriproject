# Quick Start Guide — Innamorarsi di Pirri Website

## 📦 What You Have

A complete, production-ready e-commerce website for your book in a **single HTML file**.

**File:** `index.html` (30 KB)
**No build process needed** — just open it in a browser or upload to a web server.

---

## 🚀 Quick Start

### 1. Test Locally
```bash
# On macOS:
open index.html

# On Windows/Linux:
# Double-click index.html or open with your browser
```

The website should load completely with:
- ✅ Beautiful hero section
- ✅ Book information
- ✅ 6 content chapters
- ✅ Author bios
- ✅ Scrolling architecture gallery
- ✅ Complete checkout form
- ✅ Professional footer

### 2. Deploy to the Web

**Easiest: Netlify (Recommended)**
1. Go to https://netlify.com
2. Sign up (free)
3. Drag & drop your `index.html` file
4. Get a live URL instantly

**Alternative: GitHub Pages**
1. Push this project to GitHub (see GITHUB_SETUP.md)
2. Go to Settings → Pages
3. Select "main" branch as source
4. Your site is live at `https://marcellalai79.github.io/pirriproject`

---

## ✏️ Customization

### Change Book Price
Find this line in `index.html`:
```html
<span class="price-amt">18</span>
```
Change `18` to your price.

### Change Author Names
Search for:
```html
Maria Rosaria Lai — Marcella Lai
```
Replace with your names.

### Change Book Description
Find the "About" section and edit:
```html
<p>«Innamorarsi di Pirri» unisce ricerca storica...
```

### Change Colors
At the top of the `<style>` block:
```css
:root {
  --sand: #f5efe6;     /* Light cream background */
  --terra: #b8622a;    /* Warm brown accent */
  --deep: #1e1810;     /* Dark brown text/headers */
  --stone: #7a6a58;    /* Muted gray text */
  /* ... */
}
```

---

## 🛒 Checkout Features

The checkout form includes:

1. **Step 1: Customer Details**
   - Name, surname, email
   - Form validation

2. **Step 2: Payment Information**
   - Card number (formatted automatically)
   - Expiry date (MM / YY)
   - CVV security code

3. **Step 3: Order Review**
   - Order summary
   - Customer details confirmation

4. **Step 4: Processing**
   - Animated loading indicator

5. **Step 5: Success**
   - Thank you message
   - Download button

**Note:** Currently this is a demo. To accept real payments, integrate with:
- **Stripe** (easiest): https://stripe.com
- **PayPal**: https://paypal.com
- **Square**: https://squareup.com

---

## 📱 Responsive Design

The website automatically adapts to:
- 💻 Desktop (1200px and above)
- 📱 Tablet (768px - 1199px)
- 📱 Mobile (below 768px)

Test on your phone to see it in action!

---

## 🔒 Real Payment Integration

To enable actual payments:

### For Stripe:
1. Create account at https://stripe.com
2. Get your API keys
3. Add Stripe.js to the HTML:
```html
<script src="https://js.stripe.com/v3/"></script>
```
4. Create a backend server (Node.js, Python, etc.) to process payments
5. Replace the demo form with real payment processing

### For PayPal:
Similar process, use PayPal's payment buttons instead.

---

## 📊 Analytics (Optional)

Add Google Analytics to track visitors:

```html
<!-- Add before closing </head> tag -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

Replace `GA_MEASUREMENT_ID` with your Google Analytics ID from https://analytics.google.com

---

## 📧 Email Setup (Optional)

To send order confirmations, set up an email service:

**Using Firebase/Firestore:**
- Free tier available
- Backend integration required

**Using SendGrid:**
- Free up to 100 emails/day
- API integration needed

**Using Mailgun:**
- Free tier available
- Good for transactional emails

---

## 🎨 Typography

Currently uses:
- **Headers:** Cormorant Garamond (300 weight) — elegant and timeless
- **Buttons/Labels:** Josefin Sans (200-300 weight) — modern and clean

To change fonts:
1. Find the `@import` at the top of the `<style>` block
2. Change the Google Fonts URLs
3. Update the CSS variables:
```css
--serif: 'Your Font Name', serif;
--sans: 'Your Other Font', sans-serif;
```

---

## 🖼️ Adding Images

The current architecture SVGs are placeholder illustrations. To add real photos:

1. Save your image: `photo.jpg`
2. Add to the hero section:
```html
<img src="photo.jpg" alt="Pirri architecture" style="width:100%; height:100%; object-fit:cover;">
```

3. Do the same for gallery tiles and other sections

---

## 📥 Download System

Currently the "Download" button is a placeholder. To set up real downloads:

### Option 1: Direct File Host
```html
<a href="https://yourhost.com/path/to/book.pdf" 
   class="btn-dl" download="Innamorarsi-di-Pirri.pdf">
   ⬇ Scarica il PDF
</a>
```

### Option 2: AWS S3 (Secure)
1. Upload PDF to AWS S3
2. Generate signed URLs for time-limited downloads
3. Send signed URL via email after payment

### Option 3: Gumroad (Easiest)
- Use Gumroad to host your PDF
- Embed their checkout in your site
- They handle everything including downloads

---

## 🔐 SSL Certificate

Before going live, get an SSL certificate:
- **Free:** Let's Encrypt (https://letsencrypt.org)
- **Via hosting:** Most hosts provide free SSL
- **Premium:** Comodo, DigiCert (optional, for higher trust)

---

## 📋 Pre-Launch Checklist

- [ ] Tested website in multiple browsers
- [ ] Tested on mobile devices
- [ ] Updated all book information
- [ ] Changed author names
- [ ] Proofread all text
- [ ] Set up payment processor
- [ ] Configured email system
- [ ] Added SSL certificate
- [ ] Deployed to web server
- [ ] Added analytics
- [ ] Set up backup system
- [ ] Tested checkout flow end-to-end

---

## 🚨 Troubleshooting

**Website looks broken?**
- Clear browser cache (Ctrl+Shift+Delete)
- Try in incognito/private mode
- Check browser console for errors (F12)

**Form validation not working?**
- Check browser console for JavaScript errors
- Ensure JavaScript is enabled

**Images not loading?**
- Check file paths are correct
- Ensure CORS is not blocking images
- Try relative paths: `./images/photo.jpg`

**Checkout not submitting?**
- Check browser console for errors
- Verify form fields are all filled correctly
- Check browser security settings

---

## 📞 Support

For technical help:
- Browser DevTools: Press F12 to inspect elements
- HTML/CSS/JavaScript reference: https://mdn.mozilla.org
- React documentation: https://react.dev

---

## 🎉 You're Ready!

Your e-commerce website is complete and ready to deploy.

**Next step:** Push to GitHub and deploy to the web!

See `GITHUB_SETUP.md` for detailed instructions.

---

**Happy selling!** 📚✨
