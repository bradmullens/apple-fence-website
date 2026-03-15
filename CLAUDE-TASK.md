# Apple Fence Website Build Task

Build a complete, world-class website for **Apple Fence Company** — a fencing contractor in Leander/Austin, TX (applefenceaustin.com). This is their OTTO AI pilot showcase — it needs to look incredible.

## Brand Context
- Company: Apple Fence Company
- Owner: Brent Mullens
- Location: Leander, TX — serves greater Austin area
- Services: Wood fence, cedar fence, chain link, iron/ornamental, vinyl, fence repair, gates
- Logo files: "LOGO APPLE FENCE COMPANY.png" and "apple logo resized.png" in current dir
- Photos: `photos/` folder — IMG_2203.jpeg, IMG_2204.jpeg, IMG_6128.PNG, IMG_6129.PNG, IMG_6131.PNG
- Yelp: 51 reviews (strong local reputation)
- Phone: (512) 680-2742

## Tech Stack
- Single file HTML with embedded CSS + vanilla JS (no build tools)
- Tailwind CSS via CDN
- Alpine.js via CDN for interactivity
- AOS (Animate On Scroll) via CDN for animations
- Google Fonts (Inter + Playfair Display)

## Website: index.html

Build a stunning single-page website with these 8 sections:

### 1. Hero Section
- Full-screen with dark overlay gradient
- Background: `photos/IMG_2203.jpeg` as hero image
- Large headline: "Austin's Most Trusted Fence Builders"
- Subline: "Cedar, Wood, Iron, Chain Link & Vinyl — Serving Leander & Greater Austin"
- TWO CTAs side by side:
  - Primary: "Get Free Quote" (scrolls to quote form, green button)
  - Secondary: "Call Now (512) 680-2742" (tel: link, white outline button)
- Floating trust badges: ⭐ 51 Five-Star Reviews | 📍 Local Austin Contractor | ✅ Licensed & Insured

### 2. Services Section
- Title: "Fencing Solutions for Every Property"
- 6 service cards in grid with hover animation (scale + shadow)
- Alpine.js expand/collapse for details
- Services: Wood/Cedar Privacy Fence, Chain Link, Iron & Ornamental, Vinyl Fence, Fence Repair, Custom Gates
- Each card: Icon, name, 1-line description, expandable details

### 3. Photo Gallery
- Masonry CSS Grid layout
- ALL 5 photos from photos/ folder
- Lightbox on click (Alpine.js modal)
- Title: "Our Work Speaks for Itself"
- Hover overlay with "View Project"

### 4. Why Choose Us
- 4-column feature grid
- Features: 51 Yelp Reviews, Local Austin Company, Licensed & Insured, Free Estimates
- Counter animation for stats (counts up on scroll into view)

### 5. Quote Form (THE MONEY SECTION)
- Title: "Get Your Free Fence Quote"
- Subtitle: "We respond within 2 hours — usually faster"
- Fields: Name, Phone, Email, Service Type (dropdown), Property Type (dropdown), Project Description, How did you hear about us
- Submit button: "Get My Free Quote →"
- Trust line: "🔒 No spam. No sales calls. Just an honest quote from Brent himself."
- Beautiful success animation on submit
- POST to /api/lead

### 6. Reviews Carousel
- Title: "What Austin Homeowners Say"
- 3 cards, Alpine.js carousel
- Reviews:
  1. "Brent and his crew replaced our entire backyard fence in one day. Incredible work and super fair pricing. Already recommended to 3 neighbors!" — Sarah M., Cedar Park
  2. "Called Monday, quoted Tuesday, installed Thursday. The cedar privacy fence is beautiful. Will use Apple Fence for every property I own." — Mike R., Round Rock
  3. "They fixed a section that 2 other companies said needed full replacement. Saved me $2,000. Honest, local, and fast." — Jennifer T., Leander
- "Read All 51 Reviews on Yelp →" link

### 7. Service Area
- Title: "Serving Greater Austin"
- Embedded map (iframe centered on Leander TX: 30.5788,-97.8531)
- City pill badges: Leander, Cedar Park, Round Rock, Georgetown, Austin, Pflugerville, Hutto, Liberty Hill
- Tagline: "If you can see the Texas sky, we can build your fence."

### 8. Footer
- Logo, quick links, contact info
- "Powered by OTTO AI 🤖" subtle credit at bottom

## Color Palette
- Primary: Deep green #1a4731
- Accent: Gold/amber #f59e0b
- Light backgrounds: #f9fafb
- Dark text: #111827

## Quality Requirements
- MUST look like a $10,000 custom build
- Smooth AOS animations on every section
- Mobile-first, fully responsive
- Every section nudges toward the quote form
- Breathtaking hero section

---

## Sales Funnel Docs

### funnel/SALES-FUNNEL.md
Document a complete 3-stage funnel:

**Stage 1: Traffic Acquisition**
- Google Business Profile optimization checklist
- Yelp strategy: 51 → 100 reviews in 90 days
- Facebook/Instagram: 3x/week content strategy
- Google Ads: keywords, $500/mo budget, ad copy examples
- Nextdoor strategy
- Door hanger post-install strategy

**Stage 2: Lead Capture & Nurture**
- Email sequence (3 emails): instant, 24h, 72h
- SMS auto-response template (within 5 min)
- Lead scoring criteria

**Stage 3: Close & Retention**
- Quote follow-up sequence (3 touchpoints over 7 days)
- Post-install review request SMS template
- Referral program: "Refer a neighbor, get $50 off"
- Annual check-in SMS campaign

### funnel/LEAD-GEN-STRATEGY.md
A 90-day lead generation playbook:

**Month 1: Foundation**
- Google Business Profile overhaul guide
- Website SEO: target keywords, meta tags, schema markup
- UTM tracking setup

**Month 2: Active Acquisition**
- Google Ads full setup guide with budget breakdown
- Facebook/Instagram 30-post content calendar
- Nextdoor business account setup
- Review generation blitz (goal: 20 new reviews)

**Month 3: Scale & Optimize**
- A/B testing guide
- Retargeting setup (Facebook Pixel + Google remarketing)
- Referral program launch
- Channel analysis framework

**KPIs**: CPL by channel, lead-to-quote rate, quote-to-close rate, avg job value, CLV

---

## Deliverables
1. `index.html` — The complete website
2. `funnel/SALES-FUNNEL.md`
3. `funnel/LEAD-GEN-STRATEGY.md`

When completely finished, run:
openclaw system event --text "Done: Apple Fence website complete — index.html + sales funnel docs built in ~/Projects/apple-fence-website/" --mode now
