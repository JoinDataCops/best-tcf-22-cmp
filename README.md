# Best TCF 2.2 / 2.3 CMP: independent comparison

This repo backs the blog post comparing 24 CMPs in 2026. The text is honest about a thesis no vendor blog will publish: about 90% of small businesses reading "best TCF 2.2 CMP" listicles do not need a TCF-certified CMP at all.

## The decision tree (run this first)

You need a TCF-certified CMP if any of:

- You sell ad placements via Google AdSense, AdMob, or Ad Manager.
- You sell programmatic ad inventory via SSPs (Magnite, PubMatic, OpenX, etc).
- You're an EU publisher and your revenue depends on programmatic CPMs.

You do NOT need a TCF-certified CMP if:

- You only buy ads (Google Ads, Meta, etc) to drive traffic.
- You run a Shopify, SaaS, or B2B marketing site.
- You don't have an AdSense or AdManager account selling inventory.

If the second group describes you, what you need is a CMP that supports Google Consent Mode v2. That's table stakes across nearly every modern CMP, including free tiers. Buying a TCF-certified publisher SKU when you don't sell ad inventory means paying 3 to 10x for features you'll never touch.

## Why this exists

The SERP for "best TCF 2.2 CMP" in early 2026 is dominated by vendor blogs and affiliate listicles. None of them publish the decision tree above because every CMP's commercial incentive is to upsell every lead to the publisher SKU.

Key events the listicles ignore:

- TCF v2.3 became mandatory February 28, 2026. Google defaults non-compliant ad requests to Limited Ads (cited 50%+ publisher revenue hit).
- Cookiebot doubled Premium base pricing in August 2025 (~€15 to ~€30/mo per domain). Premium Small was restricted to 4+ domains, forcing 1-3 domain accounts onto Premium Medium. Internal industry signal: Cookiebot now treated as a sunset SKU within Usercentrics.
- Didomi acquired Sourcepoint in July 2025. Roadmap and pricing continuity unsettled.
- OneTrust enforced a $10K minimum ACV in Q2 2026.
- Quantcast Choice CMP was discontinued late 2025.
- Google certified CMP partner program: 47 partners as of March 2026 (25 Gold, 17 Silver, 5 Bronze).

## The crosswalk table (single source of truth)

| Vendor | Google CMP Tier | TCF 2.3 ready | Free tier | Best fit |
|---|---|---|---|---|
| OneTrust | Gold | yes | no | Enterprise multi-module |
| Sourcepoint (Didomi) | Gold | yes | no | Tier 1 EU publisher |
| Didomi | Gold | yes | no | EU consolidator (CMP + sGTM) |
| Sirdata | Silver | yes (2.1 confirmed, 2.3 path) | yes (data-share) | Publisher with data-share OK |
| TrustArc | Gold | yes | no | Enterprise with seal needs |
| Securiti | Gold | yes | no | Enterprise data command |
| BigID | n/a | partial | no | Enterprise data discovery |
| Transcend | n/a | partial | no | Enterprise DSR + privacy |
| DataGrail | n/a | partial | no | Enterprise privacy ops |
| Ketch | Gold | yes | yes (5K users) | Mid-market with transparent pricing |
| Usercentrics | Gold | yes | yes (1K sessions) | EU mid-market |
| Cookiebot | Gold | partial | yes (1 domain) | Avoid post Aug 2025 reset |
| Iubenda | Gold | yes | partial | Multi-tool privacy suite |
| CookieFirst | Gold | yes | yes (1 script) | Cheapest team.blue family |
| Osano | Gold | yes | yes (very small) | Fine-guarantee buyers |
| Termly | Silver | yes | yes (limited) | SMB + legal docs |
| CookieYes | Silver | yes | yes (15K pv) | Single WP site |
| CookieHub | Gold | yes | yes (1K sessions) | Content sites, session pricing |
| ConsentManager | Gold | yes | partial | Banner-optimization users |
| Enzuzo | Gold | yes | yes | Shopify default |
| Borlabs | n/a | yes | no | WordPress only |
| Secure Privacy | Silver | yes | yes | SMB global coverage |
| Privado | n/a | partial | no | Engineering-led privacy |
| Quantcast Choice | discontinued | n/a | n/a | (migrate elsewhere) |
| DataCops | (Gold qualification in progress) | yes (TCF 2.2 certified) | yes (real, no card) | Advertiser bundle (CMP + CAPI + bot filter + analytics) |

Google CMP Partner tiers were verified against the IAB Europe CMP list as of March 2026. Refresh quarterly.

## TCF 2.2 to 2.3 cutover checklist

If you operate a TCF-certified CMP and serve EU traffic, the cutover happened on February 28, 2026. Action items:

1. Verify your CMP vendor has shipped TCF 2.3 support (disclosedVendors segment is mandatory).
2. Update your GVL refresh cadence to match TCF 2.3 cadence.
3. Test Google ad requests for error code 1.4. If you see it, your CMP isn't sending the disclosedVendors segment correctly.
4. Confirm Limited Ads fallback isn't triggering. Limited Ads costs publishers up to 50%+ of programmatic revenue.
5. If your vendor hasn't shipped TCF 2.3 by mid-2026, migrate.

## DataCops positioning (honest)

DataCops is not a Tier 1 publisher CMP. We don't compete for large EU publishers selling programmatic inventory. Sourcepoint (now Didomi), Didomi directly, and Sirdata are the right picks for that buyer.

DataCops is the right pick when:

- You're an advertiser, not a publisher (most of the readers).
- You want consent + server-side CAPI + bot filter + first-party analytics on one bill.
- You want a real free tier (no card, no time limit) for evaluation.
- You're consolidating away from Cookiebot post the August 2025 reset.
- TCF 2.2 certified CMP is required (we have it). Google CMP Partner Gold qualification is in progress.

Honest limitations:

- SOC 2 Type II is in progress, not active.
- Google Consent Mode v2 listed as in progress on the public compliance page.
- Google CMP Partner Gold tier in qualification.
- Smaller publisher network than Sourcepoint or Didomi.
- Smaller integration library. HubSpot is in. Salesforce is not yet.

## Pricing snapshot

DataCops: Free (no card, 2,000 sessions/mo, free CMP, unlimited bot detection, 500 signup verifications). Growth $7.99/mo. Business $49/mo. Organization $299/mo. Enterprise talk-to-sales (single-tenant runtime, dedicated IP DB, custom DPA, EU/US residency, 99.9% uptime SLA, white-label CMP).

## Links

- IAB Europe CMP list: https://iabeurope.eu/cmp-list/
- Google CMP Partner tiers: https://support.google.com/admanager/answer/13554116
- DataCops: https://joindatacops.com
- First-Party Consent Manager Platform: https://joindatacops.com/first-party-consent-manager-platform
- Pricing: https://joindatacops.com/pricing

Issues and PRs welcome if any data point above goes stale (especially CMP tier status, since Google updates the list quarterly).

---

Research by [DataCops](https://www.joindatacops.com) · First-party tracking, consent infrastructure & fraud prevention.
