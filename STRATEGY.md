# Triberr Distribution Strategy

## 1. Business Model: Zero Commission, Ecosystem Monetization

No commission ever. The agent keeps 100% of every rupee collected via GPay/UPI. Platform never touches customer payments.

**Revenue streams:**
- **App installs during visits** -- Agents install partner apps (fintech, edtech, ecommerce) during home visits. Per-install payouts from partners. This is the killer monetization: physical distribution at scale.
- **Page-level ads** -- Each expert's service page carries contextual ads (local businesses, SaaS tools, ISPs). CPM/CPC model.
- **Certification fees** -- Paid training tracks (cybersecurity, smart home, AI tools). Certified experts get a badge + priority listing. Rs 999-2999/track.
- **SaaS tier** -- Free tier is permanent. Premium: analytics dashboard, CRM, lead routing, auto-scheduling, branded domain. Rs 299/mo.
- **Brand partnerships** -- Hardware brands pay for "Recommended by Triberr" shelf placement during visits. Commission on hardware sold through expert referral links.

Think Meesho for tech services: empower the last-mile agent, monetize the network.

## 2. Anti-Disintermediation: Why They Stay

- **Zero commission = zero reason to leave.** There is no middleman fee to bypass.
- **Platform gives, never takes:** branded page, search discovery, Google indexing, verified trust badge, training content.
- **Ratings are non-portable.** Leave Triberr, lose your 4.8-star reputation built over 50+ visits.
- **Customer trust is institutional.** Customers book "a Triberr expert," not a freelancer. The badge is the brand.
- **Network effects compound.** Top-rated experts get more visibility. New experts need the platform to bootstrap trust.

## 3. Rating System

Post-visit flow:
1. Expert marks visit complete in dashboard
2. Customer receives WhatsApp message with feedback link (auto-sent via WhatsApp API)
3. Simple form: 1-5 stars + optional comment (under 30 seconds)
4. Rating appears publicly on expert's page

**Quality control:**
- Below 3.5 stars (rolling 10 visits): yellow warning, tips sent
- Below 3.0 stars: delisted, must complete retraining to re-activate
- Fraud detection: flag if expert requests specific ratings

## 4. Distribution Architecture

**Single-file fork model:**
```
config.js: { name, whatsapp, city, photo, bio, services[] }
```

- **Routes:** `triberr.in/rahul` or `?expert=rahul` on GitHub Pages
- **Central registry:** `experts.json` -- array of all active expert configs, fetched by main site for discovery/search
- **Onboarding:** Fill a Google Form -> auto-generates config -> PR merged -> page live in <24hrs. Later: self-serve dashboard.
- **Tech stack stays static.** No backend needed until 100+ experts. GitHub Pages + JSON + WhatsApp API.

## 5. Growth Flywheel

```
Recruit local expert -> Give them a branded page -> They do doorstep visits
-> Customer rates them -> Ratings build trust -> Page ranks on Google
-> More customers find them -> Expert earns more, stays loyal
-> Expert recruits other experts in their city -> Network expands
```

**Ignition strategy:** Seed 5 experts in 3 cities. Each does 10 visits/week. 150 rated visits in month one. Those pages rank locally. Organic inbound begins. Flywheel turns.

**Viral loop:** Every WhatsApp message ("Your Triberr expert Rahul is on the way") is free brand distribution to the customer's phone.
