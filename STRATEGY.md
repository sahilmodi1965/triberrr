# Triberr — Platform Strategy & Architecture

## Vision

Triberr is digital infrastructure for India. Not a gig marketplace — a **distribution network** where ground agents deliver tech literacy, app adoption, and digital transformation to every doorstep. Think of each Triberr expert as a human API between India's digital economy and the 500M+ people who need a hand getting on board.

---

## 1. Business Model: Zero Commission, Distribution Monetization

**The expert keeps 100% of every rupee.** Platform never touches customer payments. Experts collect via GPay/UPI/cash directly.

This is non-negotiable. Commission creates adversarial incentives. Zero commission creates loyalty.

### Platform revenue streams (in order of priority):

| Stream | How it works | Revenue model |
|--------|-------------|---------------|
| **Affiliate links** | Every app/tool set up during a home visit earns Triberr a referral fee. Expert installs Zerodha, Cred, Notion, Canva, hosting providers, etc. — tracked via affiliate link. | Per-install / per-signup payout |
| **Adoption partnerships** | Brands pay Triberr to not just *install* but *fully adopt* their app. Expert trains the customer, sets up the account, does first transaction. Verified adoption > verified install. | Premium per-adoption fee (3-10x of install) |
| **App distribution campaigns** | Run promotional campaigns: "This month, set up 50 Google Business Profiles in your area." Brand pays per completed setup. Expert earns a bonus. Platform earns campaign fee. | Campaign management fee + per-unit |
| **SaaS premium tier** | Free forever for basic. Premium: analytics dashboard, CRM, lead routing, auto-scheduling, branded subdomain. | ₹499/mo per expert |
| **Certification & training** | Paid tracks: cybersecurity, smart home, AI tools, business digitization. Certified = trust badge + priority listing. | ₹1,999-4,999/track |
| **Page-level contextual ads** | Each expert's page carries relevant local ads (ISPs, hardware stores, coaching centers). | CPM/CPC |
| **Consulting revenue share** | For large projects (website builds, full shop digitization, CRM), platform provides backend support and shares in project fee. | 15-20% on projects > ₹5,000 |

### Why this is bigger than a gig platform:
- Swiggy/Zepto AOV: ₹300-500. **Triberr AOV: ₹999-2,999.**
- A food delivery is a transaction. A Triberr visit is a **relationship** — the expert becomes the family/shop's trusted tech person.
- Every visit is a distribution opportunity. 1 home visit = 3-5 app installs = ₹150-500 in affiliate revenue on top of the service fee.

---

## 2. Expert Economics: ₹30K/month Minimum Target

### The math:
| Metric | Value |
|--------|-------|
| Working days/month | 25 |
| Visits/day | 2-3 |
| Avg service fee | ₹999 |
| Monthly service income | ₹49,950 - ₹74,925 |
| Affiliate bonus/visit | ₹100-200 |
| Monthly affiliate income | ₹5,000 - ₹15,000 |
| Campaign bonuses | ₹2,000 - ₹5,000 |
| **Total monthly earning** | **₹57,000 - ₹95,000** |
| **Floor (conservative: 1.5 visits/day, ₹799 avg)** | **₹32,963** |

The ₹30K floor is achievable with just 1.5 visits/day at modest pricing. Top performers will clear ₹80K+.

### Expert tiers:
- **Starter** — 0-25 visits. Learning phase. Access to all basic services.
- **Verified** — 25+ visits, 4.0+ rating. Gets trust badge, priority in local search.
- **Pro** — 100+ visits, 4.3+ rating. Access to premium campaigns, higher affiliate rates, branded subdomain.
- **Champion** — 250+ visits, 4.5+ rating. Can recruit & mentor new experts. Earns referral bonus per recruit.

---

## 3. Anti-Disintermediation: Why Experts Never Leave

| What they'd lose | Why it matters |
|-----------------|---------------|
| ₹0 commission | No financial incentive to bypass |
| Ratings (non-portable) | 4.8 stars built over 100 visits — gone if they leave |
| Trust badge | Customers book "a Triberr expert" not a freelancer |
| Affiliate income | They can't get Zerodha/Cred affiliate links on their own easily |
| Campaign access | Promotional campaigns = bonus income they can't source independently |
| Google ranking | Their Triberr page ranks for "[city] laptop setup" — their personal page won't |
| Training & certification | Skills they got through Triberr |
| Community | Network of experts to learn from, refer overflow work |

**The platform gives everything and takes nothing from the service fee.** There is literally no reason to leave.

---

## 4. Rating & Quality System

### Post-visit flow:
1. Expert marks visit complete (WhatsApp message to admin: "DONE | Customer: [name] | Service: [x]")
2. Customer receives WhatsApp feedback link (auto or manual)
3. Simple form: 1-5 stars + optional comment (< 30 seconds)
4. Rating appears on expert's public page

### Quality thresholds:
- **4.0+ stars** → Verified badge
- **3.5-4.0** → Normal, no badge
- **Below 3.5 (rolling 10 visits)** → Yellow warning + improvement tips
- **Below 3.0** → Temporarily delisted. Must complete retraining to reactivate.
- **Fraud detection** → Flag if expert requests specific ratings or reviews look templated

### Customer protection:
- Every booking is logged (WhatsApp thread = audit trail)
- Customers can escalate to Triberr admin via WhatsApp
- "Satisfaction guarantee" badge for Pro/Champion experts

---

## 5. Affiliate & Distribution Architecture

### How affiliate links work during a home visit:

```
Customer books "New laptop setup" (₹999)
→ Expert visits home
→ Sets up laptop
→ During setup, installs recommended apps via Triberr affiliate links:
   - Browser: Brave (affiliate)
   - Password manager: 1Password (affiliate) 
   - Cloud: Google One (affiliate)
   - Finance: Zerodha/Groww (affiliate)
   - Shopping: Amazon (affiliate)
   - Productivity: Notion (affiliate)
→ Each install tracked to expert
→ Platform earns ₹30-200 per install
→ Expert gets nothing deducted — affiliate is pure platform revenue
```

### Campaign model:
```
Brand: "Google wants 10,000 Google Business Profiles set up in Tier 2 cities"
→ Triberr creates campaign: "Set up Google Business Profile — ₹349 to customer, ₹200 bonus to expert per setup"
→ Experts in 50 cities run the campaign
→ Google pays Triberr ₹500/setup
→ Triberr keeps ₹300, expert gets ₹200 bonus (on top of ₹349 service fee)
→ Expert earns ₹549 per visit. Customer gets expert help for ₹349.
→ Google gets verified adoption, not just a download.
```

**This is the killer insight: brands pay 10x for verified adoption vs. an app install ad.** Triberr experts don't just install — they train, onboard, and ensure the customer actually uses the product.

---

## 6. Platform Evolution Roadmap

### Phase 1: GitHub Pages (NOW)
- Single HTML file per expert, config-driven
- WhatsApp-based booking and feedback
- Manual onboarding (Google Form → config → page live)
- Track everything via WhatsApp threads
- Goal: 50 experts, 5 cities, 1,000 visits

### Phase 2: Central Platform (Month 3-6)
- `triberr.in/rahul` — expert subdomains
- Central expert directory with search by city/service
- `experts.json` registry — API for all active experts
- Admin dashboard: see all visits, ratings, affiliate conversions
- Automated feedback links via WhatsApp Business API
- Goal: 200 experts, 15 cities, 5,000 visits/month

### Phase 3: Customer App (Month 6-12)
- Customer downloads Triberr app (or PWA)
- Browse experts by location/rating/specialty
- Book consultation or service package
- **Home visit is mandatory** — no remote-only option. The doorstep visit IS the product.
- Package booking: "Family Digital Setup Day" (bundle of 5 services at discount)
- In-app payment (optional, expert can still accept GPay/cash)
- Push notifications for campaign promotions
- Goal: 500 experts, 30 cities, app installs via ground experts

### Phase 4: Distribution Platform (Month 12+)
- Triberr becomes the **ground distribution layer** for India's digital economy
- Any SaaS, fintech, edtech, healthtech company can run adoption campaigns through Triberr
- Expert marketplace: companies bid for expert time during visits
- AI-powered visit optimization: "While you're setting up their laptop, also offer Google Workspace — they're a freelancer"
- Expert earnings dashboard with affiliate attribution
- **Triberr is to digital adoption what Meesho is to e-commerce: the last-mile human layer.**

---

## 7. Competitive Moat

1. **Ground truth data** — We know what apps every household uses, what they struggle with, what they'll pay for. This data is gold for product companies.
2. **Trust network** — Rated, verified experts in every neighbourhood. Takes years to build, impossible to replicate overnight.
3. **Adoption > Install** — Our experts ensure real usage, not just downloads. This is 10x more valuable to brands.
4. **Zero commission loyalty** — Experts have no reason to leave. Every other platform takes 20-30%. We take 0%.
5. **Physical distribution** — In a world of digital ads with 0.5% CTR, a trusted person at your door has 90%+ conversion.

---

## 8. The Triberr Equation

```
For the Expert:    ₹30K-90K/month + skill building + community
For the Customer:  Trusted tech help at their doorstep
For the Platform:  Affiliate revenue + campaign fees + data + distribution power
For Brands:        Verified adoption at scale, not just impressions

Everyone wins. Nobody is exploited. India gets digitized.
```
