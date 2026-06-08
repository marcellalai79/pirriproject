# Innamorarsi di Pirri — E-Commerce Website

A beautiful, editorial-style e-commerce website for the book "Innamorarsi di Pirri: Bellezze d'architettura e d'arte" by Maria Rosaria Lai (text) and Marcella Lai (photography).

## Features

✨ **Modern Design**
- Elegant serif typography (Cormorant Garamond, Josefin Sans)
- Sophisticated color palette inspired by Sardinian architecture
- Fully responsive layout

🛒 **E-Commerce**
- Complete checkout flow with multi-step form
- Form validation
- Order summary and review
- Payment processing simulation

📖 **Content Sections**
- Hero section with book introduction
- About section with book mockup
- Six content chapters
- Scrolling gallery of architectural photography
- Author bios
- Shop with detailed product features
- Professional footer

⚙️ **Technology**
- Single-file HTML5 application
- React 18 (via CDN)
- No build process required
- Works in all modern browsers

## Book Details

**Title:** Innamorarsi di Pirri — Bellezze d'architettura e d'arte

**Authors:**
- Maria Rosaria Lai (Text & Historical Research)
- Marcella Lai (Photography & Visual Curation)

**Format:** Digital PDF, 240 pages

**ISBN:** 979 12 80117 00 7

**Publisher:** Edizioni Domus de Janas, Sestu (CA)

**Year:** 2020

**Price:** €18

## Content Overview

### Chapters
1. **L'Antica Periferia** — Country houses, villas & rural estates
2. **Il Centro Storico** — Urban structure and Campidanese architecture
3. **Arte Sacra** — Churches and religious heritage
4. **Il Novecento** — Art Nouveau & modern architecture
5. **Ville & Palazzi** — Noble and bourgeois residences
6. **Apparati** — Preface, historical notes, archival sources

## File Structure

```
pirri-project/
├── index.html          # Main website (single-file, includes all CSS & JS)
├── README.md          # This file
├── LICENSE            # Project license
└── assets/            # (For future PDF download link, images, etc.)
```

## Installation & Deployment

### Local Testing
Simply open `index.html` in any modern web browser:
```bash
# macOS
open index.html

# Linux/Windows
# Double-click index.html or open with your browser
```

### Deploy to Web
1. Upload `index.html` to your web host
2. No server-side processing required for the demo
3. For real payment processing, integrate with a payment provider (Stripe, PayPal, etc.)

## Customization

### Colors
Edit the CSS variables in the `<style>` block:
```css
:root {
  --sand: #f5efe6;
  --terra: #b8622a;
  --deep: #1e1810;
  --stone: #7a6a58;
  /* ... */
}
```

### Content
All text content can be edited directly in the HTML file. Search for text to find sections to modify.

### Payment Integration
The checkout form is currently a demo. To enable real payments:
1. Integrate with Stripe, PayPal, or another payment processor
2. Add backend server logic to handle payment processing
3. Generate and send download links upon successful payment

## Features in Detail

### Checkout Flow
1. **Customer Details** — Name, email, country
2. **Payment Information** — Card number, expiry, CVV
3. **Order Review** — Summary of purchase
4. **Processing** — Payment animation
5. **Success** — Download link generation

### Responsive Design
The website is fully responsive and works on:
- Desktop (1200px+)
- Tablet (768px - 1199px)
- Mobile (< 768px)

### Accessibility
- Semantic HTML structure
- Clear typography hierarchy
- Good color contrast
- Keyboard navigation support

## Browser Support

- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Mobile Safari 14+
- Mobile Chrome

## License

This website design and code are created for the "Innamorarsi di Pirri" book project.

All photography and text content in the book © Maria Rosaria Lai & Marcella Lai, 2020.

## Contact

- **Publisher:** Edizioni Domus de Janas
- **Email:** domusdejanaseditore@tiscali.it
- **Location:** Sestu (CA), Sardegna, Italia

## Next Steps

### To Make This Production-Ready:
1. ✅ Design complete
2. ⬜ Integrate real payment processor (Stripe/PayPal)
3. ⬜ Set up PDF delivery system
4. ⬜ Add analytics (Google Analytics, etc.)
5. ⬜ Set up SSL certificate
6. ⬜ Deploy to web hosting
7. ⬜ Add email confirmation system
8. ⬜ Implement order tracking

---

**Website Created:** May 2026  
**Last Updated:** May 29, 2026
