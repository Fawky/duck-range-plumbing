# Duck Range Plumbing and HVAC Ltd. — Project Context

## Client

**Business:** Duck Range Plumbing and HVAC Ltd.
**Owner:** Chris
**Phone:** 250-214-0539
**Address:** 197 Shuswap Avenue, Chase, BC V0E 1M0
**Service area:** Chase, Pritchard, Sorrento & North Shuswap
**Live site:** https://duck-range-plumbing.pages.dev/
**GitHub repo:** https://github.com/Fawky/duck-range-plumbing (public)
**Facebook:** https://www.facebook.com/p/Duck-Range-Plumbing-Heating-LTD-61577103894593/
**Yellow Pages:** https://www.yellowpages.ca/bus/British-Columbia/Chase/Duck-Range-Plumbing-and-HVAC-Ltd/101886689.html
**Hours:** Mon–Fri 9:00am–5:30pm
**Experience:** 16 years industry experience
**Credentials:** Licensed & Insured · Gas Fitting Certified (BC) · Free Quotes

---

## Project Brief

Build a premium, production-ready single-page website for a local owner-operated plumbing and HVAC business in Chase, BC. Client provided logo only — all copy and photos sourced from Yellow Pages, Facebook, and the Bree-Link project's photo library.

**Design rules (strictly enforced):**
- No emojis — inline SVG icons only
- All CSS inline in `<style>` block; Google Fonts the only external resource
- Mobile-first: `clamp()` typography, `@media (max-width:768px)` stacked layouts, 44px min touch targets
- Animations: `@keyframes fadeInUp` on hero load, `IntersectionObserver` scroll reveal
- Fonts: Montserrat (headings 600/700), Open Sans (body 400/600)
- Spacing scale (4px base): 4 8 12 16 24 32 48 64 96 128px
- Footer: `© <span id="yr"></span> Duck Range Plumbing and HVAC Ltd. · Design by Steep Creative`
- `index.html` is the active site — based on Bree-Link layout structure

---

## Files in This Folder

| File | Description |
|---|---|
| `index.html` | **Active homepage** — Bree-Link layout adapted for Duck Range |
| `logo.png` | Client logo — 1438×616px RGBA PNG, black flying duck silhouette + wordmark on transparent bg |
| `favicon.svg` | SVG favicon — flying duck silhouette on navy rounded square |
| `context.md` | This file |
| `v1-navy-copper.html` | Design variant — Deep Navy & Copper |
| `v2-forest-stone.html` | Design variant — Forest Green & Stone |
| `v3-blue-cream.html` | Design variant — Warm Blue & Cream |
| `v4-charcoal-amber.html` | Design variant — Charcoal & Amber |

### site-images/
| File | Description |
|---|---|
| `hero.jpg` | Hero background photo |
| `service-residential.jpg` | Plumbing Repairs card |
| `service-hotwater.jpg` | Heating & Furnace card |
| `service-gasfitting.jpg` | Gas Fitting card + About section photo |
| `service-commercial.jpg` | Irrigation Systems card |
| `service-emergency.jpg` | Water Treatment card |
| `service-drains.jpg` | Drain & Sewer card |

---

## Homepage Sections (index.html)

1. **Top bar** — fixed, navy; location + service area left; phone number + "Get a Free Quote" CTA right (CTA hidden on mobile)
2. **Sticky header / nav** — Duck Range logo, desktop nav links, "Call Now" CTA; checkbox hamburger menu on mobile (no JS)
3. **Hero** — cert pills (Licensed & Insured, 16 Years Experience, Free Quotes); H1; subheadline; primary/secondary CTAs; trust row; quote form card (Name, Phone, Email, Service dropdown)
4. **Services** — 6 cards with photos: Plumbing Repairs, Heating & Furnace, Gas Fitting, Irrigation Systems, Water Treatment, Drain & Sewer
5. **Testimonials** — 3 reviews (Sarah M./Chase, Dave L./Sorrento, Marlene T./Pritchard)
6. **About** — Chris bio + trust badges (licensed, 16 yrs, gas fitting, free quotes); gas fitting photo right
7. **Gallery** — dark section; 3×2 grid of 6 service photos
8. **FAQ** — 8 accordion items (`<details>` + JS smooth animation)
9. **Contact** — address, phone, email, hours, Facebook link left; contact form right
10. **Footer** — 4-col grid (brand, quick links, services, contact) + © year JS + Design by Steep Creative

**Schema / meta:**
- `LocalBusiness` + `Plumber` JSON-LD schema with address, hours, areaServed
- `FAQPage` JSON-LD schema (3 Q&A pairs)

---

## Design System

```css
--blue-900:    #0B2C6B   /* deep navy — topbar, footer, hero overlay */
--blue-700:    #1B5FAF   /* hover states */
--blue-600:    #2272D4   /* primary CTA buttons, links */
--blue-100:    #E8F0FB   /* light accent bg */
--copper-600:  #C4622D   /* secondary CTA, topbar button, form submit */
--copper-700:  #A34E22   /* copper hover */
--copper-100:  #FDF0E8   /* about section bg */
--neutral-900: #1A1F2E
--neutral-700: #3D4557
--neutral-400: #8A93A8
--neutral-200: #E2E6EF
--neutral-100: #F5F6FA
```

---

## Status

- [x] 4 homepage design variations built (v1–v4)
- [x] v5 Breelink-layout version built as `index.html`
- [x] GitHub repo created (public): `Fawky/duck-range-plumbing`
- [x] Deployed to Cloudflare Pages: duck-range-plumbing.pages.dev
- [x] Hero and service photos added from Bree-Link library
- [x] Gallery section filled with service photos (3×2 grid)
- [x] About section photo added
- [x] Footer logo fixed (`filter: invert(1); mix-blend-mode: screen`)
- [x] SVG favicon created and linked
- [ ] Connect custom domain once client is ready
- [ ] Replace placeholder service photos with Duck Range's own job photos
- [ ] Add Chris's photo to About section
- [ ] GEO audit
- [ ] Landing pages (e.g. Emergency Plumbing Chase, Furnace Repair Shuswap)
