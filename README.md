# Best TCF 2.2 CMP in 2026 (and the question most listicles refuse to ask)

Let's be real. "Best TCF 2.2 CMP" is already a slightly obsolete query. TCF v2.3 became the mandatory IAB spec on February 28, 2026, with Google defaulting non-compliant ad requests to Limited Ads (cited as a 50%+ revenue hit for publishers). So the right post is "best TCF 2.2 / 2.3 CMP," and the honest version starts with a question vendor blogs will not ask: do you actually need a TCF CMP at all?

Most don't. TCF is a publisher protocol. If you sell ad placements via AdSense, AdMob, or AdManager, you need a TCF-certified CMP. If you only buy ads (run Google Ads or Meta to drive traffic to your store), Consent Mode v2 from any CMP is sufficient. About 90% of small businesses reading "best TCF 2.2 CMP" listicles do not need TCF and are being upsold a more complex product than they need.

This post is the neutral crosswalk every other listicle skips. Tools grouped by tier. /10 score per tool. Honest 4-line dossier. Decision tool at the end. Pricing where I could verify it, talk-to-sales noted where I couldn't.

---

## Quick stuff people keep asking

**Which CMPs are TCF 2.2 certified?** As of early 2026, Google lists 47 certified CMP partners across three tiers: 25 Gold, 17 Silver, 5 Bronze. The IAB Europe CMP list is the source of truth on TCF certification ID. The two lists don't perfectly overlap, which is one of the things this post tries to fix.

**What is the difference between TCF 2.2 and TCF 2.3?** TCF 2.3 became mandatory February 28, 2026. The biggest change is the disclosedVendors segment, which is now required. Google ad requests fail with error code 1.4 if the segment is missing or malformed. Limited Ads is the default fallback, which costs publishers up to 50%+ of programmatic revenue.

**Is TCF 2.2 still valid in 2026?** Technically yes, the certification doesn't expire on Feb 28. Practically no, because Google moved the goalposts and any CMP not on TCF 2.3 by now is bleeding their publisher customers' revenue.

**Do I need a TCF-certified CMP for Google Ads?** No, not if you only buy ads. Consent Mode v2 from any modern CMP is sufficient. TCF is for publishers selling ad inventory. The single most expensive misunderstanding in this category.

**Is Cookiebot TCF 2.2 certified?** Yes. Also TCF 2.3 path is on their roadmap. Note: Cookiebot doubled base pricing in August 2025, which triggered a wave of Trustpilot complaints and is the single biggest "why are we shopping for a Cookiebot alternative" trigger of 2026.

**What is the TCF vendor list?** The IAB Europe Global Vendor List (GVL). Lists every adtech vendor that's signed the TCF policy. Publishers' CMPs surface this list as the consent UI.

---

## The decision tree (read this before buying anything)

You need a TCF-certified CMP if:

- You sell ad placements via Google AdSense, AdMob, or Ad Manager.
- You sell programmatic inventory via SSPs (Magnite, PubMatic, OpenX, etc).
- You're an EU-headquartered publisher and your revenue depends on programmatic CPMs.

You do NOT need a TCF-certified CMP if:

- You only buy ads to drive traffic to your store, SaaS, or service.
- You use Meta or Google Ads for acquisition and don't sell ad inventory.
- You run a Shopify, SaaS, or B2B marketing site.

If you're in the second group, what you actually need is a CMP that supports Google Consent Mode v2, which is now table-stakes across the category. You don't need TCF certification, you don't need GVL refresh cadence, and you definitely don't need to pay enterprise CMP pricing for capabilities you'll never use.

The rest of this post still covers TCF-certified CMPs because that's the query intent. But if you skipped the decision tree and you're not a publisher, save yourself $20K to $200K and stop reading after the SMB tier.

---

## Tier 1: Enterprise / publisher-grade TCF CMPs

Full TCF 2.2 / 2.3 coverage. Built for publishers and enterprise compliance teams. Real procurement cycles.

**1. OneTrust**

The Good: Deepest module catalog in the category. Consent, DSAR, data mapping, vendor risk, PIA / DPIA, GRC, ESG. Dominant enterprise market share, the safe procurement pick.

Frustrations: 950 layoffs (25% of company) in June 2022, additional rounds reported July 2024 and June 2026. Employees and customers cite instability. Pricing opaque, new minimum $10K/year as of Q2 2026, mid-market deals $40K to $120K, enterprise $120K to $500K+. Trust has been bleeding since the 2025 PE buyout rumors.

Wish List: A flat-fee mid-market tier under $10K. Stable roadmap.

Value for Money: 6/10. The enterprise default. Worth its money only if you genuinely use 5+ modules.

Pricing: $10K/yr minimum, $40K to $500K+ ACV typical.

---

**2. Sourcepoint (acquired by Didomi July 2025)**

The Good: Deep publisher pedigree, started as anti-ad-blocking tech in 2015, grew to 200+ global enterprise customers. Strong TCF and GPP coverage. One of the most respected CMPs for publisher monetization edge cases.

Frustrations: Acquisition uncertainty, being merged into Didomi. Pricing, packaging, and roadmap continuity are unsettled. Historically expensive vs SMB CMPs, sales-led only.

Wish List: Roadmap clarity post-merger.

Value for Money: 7/10. If you're a large publisher, still a credible pick. Watch the Didomi integration carefully.

Pricing: Custom enterprise.

---

**3. Didomi**

The Good: Two big 2025 acquisitions, Addingwell (server-side tagging, April 2025) and Sourcepoint (CMP rival, July 2025) make Didomi the de facto European consolidator with CMP + sGTM under one roof. Backed by $83M Marlin Equity majority stake. Strong TCF coverage.

Frustrations: Setup complexity is the recurring complaint. Per-partner triggers in GTM, technical-level integration, multi-day implementations. Dashboard called "unintuitive" and "clunky" once you manage many policies and vendors. Admin UI hasn't kept pace with feature growth.

Wish List: Cleaner admin UI. Faster implementation path.

Value for Money: 7.5/10. The European consolidator. Right pick if you're already in their orbit and need CMP + sGTM under one roof.

Pricing: Custom enterprise.

---

**4. Sirdata**

The Good: Deeply embedded in the publisher market, 20,000+ publisher sites running ABconsent. IAB TCF v2.1 certified, well-tuned for programmatic and AdTech (per-purpose vendor management, leak prevention).

Frustrations: "Free in exchange for your data" model is a non-starter for brands with strict first-party data policies. Less brand-recognized in North America than Didomi, OneTrust, or Osano. Long US sales cycles.

Wish List: A pure paid tier without the data-share quid pro quo.

Value for Money: 6.5/10. Right for EU publishers comfortable with the model.

Pricing: Free with data exchange, paid tiers custom.

---

**5. TrustArc**

The Good: Comprehensive privacy suite covering CMP, DSR automation, PIA / DPIA assessments, global regulatory intelligence under one roof. Long history (founded as TRUSTe in 1997), deep regulatory expertise, recognized seal programs.

Frustrations: Average customer pays roughly $22K/year, enterprise deals $137K+. Pricing widely seen as inflexible. 8% pricing increases at renewal, reported by users.

Wish List: Pricing flexibility for the mid-market.

Value for Money: 6/10. Worth it for organizations with mature compliance programs that need the seal recognition.

Pricing: Avg $22K/yr, enterprise $137K+.

---

**6. Securiti**

The Good: Acquired by Veeam for $1.725B in December 2025, instantly inherits 550K+ Veeam customers and Fortune 500 distribution. True "Data Command Center" breadth: DSPM, privacy ops, AI governance, RoPA / DSAR, CMP all in one. Named a leader in major analyst rankings.

Frustrations: Pricing fully sales-led, no public floor. Module sprawl, customers report long onboarding and module-by-module licensing complexity.

Wish List: Public pricing for the SMB and mid-market entry. Tighter modular UX.

Value for Money: 8/10 if you genuinely need a Data Command Center. 6/10 if you only need a CMP.

Pricing: Custom.

---

**7. BigID**

The Good: Named a Challenger in the 2026 Gartner Magic Quadrant for Data and Analytics Governance. Industry-leading data discovery and classification across cloud, hybrid, on-prem.

Frustrations: Pricing opaque and routinely flagged as significantly higher than competitors. Clunky UI, slow performance, lengthy deployments requiring strategy formulation. Not really a CMP-first product.

Wish List: A leaner CMP-only SKU.

Value for Money: 6.5/10 for the CMP use case alone. Higher if you need full data discovery.

Pricing: Custom, quote-based.

---

**8. Transcend**

The Good: Over 1,300 pre-built integrations for data discovery and DSR automation across SaaS, data warehouses, internal systems. Recognized as a Leader in the 2025 IDC MarketScape.

Frustrations: Pricing starts around $10K/year and scales fast, outside SMB and even mid-market budgets. Custom integrations and complex SaaS connections take weeks to wire up.

Wish List: A self-serve mid-market tier.

Value for Money: 7.5/10 at the right scale. Wrong tool for SMB.

Pricing: From ~$10K/yr.

---

**9. DataGrail**

The Good: Vera AI agent (March 2026) automates PIAs / DPIAs / AI risk assessments using live system metadata. First production-ready Model Context Protocol (MCP) server for privacy. Single-tenant arch, zero external training.

Frustrations: No public pricing, every deal goes through sales. Consent module priced separately, typically +30 to 50% on ACV. Modular sticker shock at renewal.

Wish List: Bundled consent in the base SKU.

Value for Money: 7.5/10 for enterprise privacy ops. Pricing opacity hurts.

Pricing: Custom.

---

**10. Ketch**

The Good: Free tier covers up to 5K users/mo with full CMP functionality, only counts visitors not feature gating, rare in the privacy-platform space. Published transparent pricing through Plus tier ($499/mo for 100K users), no sales call until Pro / enterprise.

Frustrations: Initial setup is complex, learning curve with confusing navigation and naming conventions. Some reviewers cite poor interface design despite strong support.

Wish List: UX overhaul on initial setup.

Value for Money: 7.5/10. The pricing transparency is unusual and welcome.

Pricing: Free up to 5K users, Plus $499/mo, Pro and enterprise custom.

---

## Tier 2: Mid-market TCF CMPs

Real TCF certification, real Google CMP Partner status, prices a non-enterprise team can actually afford.

**11. Usercentrics**

The Good: Strong EU / GDPR pedigree (Munich-based) plus Cookiebot product line for SMBs after the 2021 merger. Affordable entry tiers (Essential ~€7/mo, Free up to 1,000 sessions).

Frustrations: Auto-upgrade to higher tiers when session limits are exceeded leads to surprise charges (flagged repeatedly in reviews). Inaccurate session-limit warnings and known billing bugs cited by Capterra reviewers.

Wish List: No auto-upgrade, soft limits with email notification.

Value for Money: 6.5/10. Solid product, billing surprises drag the score.

Pricing: Free up to 1,000 sessions, Essential ~€7/mo, Pro and enterprise custom.

---

**12. Cookiebot (Usercentrics-owned, sunset SKU)**

The Good: Established Usercentrics-owned CMP with broad regulator and agency familiarity. TCF v2.2 + Google CMP Partner status. Free plan covers 1 domain up to 50 subpages.

Frustrations: August 2025 pricing reset doubled Premium base from ~€15 to ~€30/mo per domain. Premium Small was restricted to 4+ domains, forcing 1 to 3 domain accounts onto Premium Medium. Effectively a 2x price hike. Wave of negative Trustpilot reviews followed. Cookiebot is now treated internally as a sunset SKU within Usercentrics.

Wish List: Roadmap clarity. The August 2025 reset feels like a managed wind-down.

Value for Money: 5.5/10. Was a 7. Pricing reset and SKU uncertainty made it a worse deal than the Tier 2 alternatives.

Pricing: Free for 1 domain / 50 subpages, Premium ~€30/mo per domain post-Aug 2025 reset.

---

**13. Iubenda (team.blue)**

The Good: Mature 360-degree privacy suite, policy generator, CMP, T&C generator, DSAR, whistleblowing, accessibility, all under team.blue. Google Gold CMP Partner (December 2024). Full Consent Mode v2 + Microsoft advertising privacy controls (July 2025).

Frustrations: Trustpilot has documented complaints about post-cancellation "threatening emails" and being told account deletion was the only way to stop them. Customer support response times stretch a week or more on lower tiers.

Wish List: Cleaner offboarding. Faster lower-tier support.

Value for Money: 7/10. Strong product, customer-relations issues drag the score.

Pricing: From €19/mo per site, plans scale.

---

**14. CookieFirst (team.blue / Iubenda)**

The Good: Google CMP Gold Partner with native Consent Mode v2, GTM integration, 44+ language auto-translated cookie policies. Cheapest serious CMP in the iubenda family: free plan for 1 script, Basic at €9/mo, Plus at €19/mo.

Frustrations: Acquired by iubenda (team.blue) in January 2025, typical post-acquisition concerns about roadmap independence and price drift. Free tier limited to 1 third-party script, most real sites need paid immediately.

Wish List: Independent roadmap commitment from team.blue.

Value for Money: 6.5/10. Cheap, certified, future uncertain.

Pricing: Free (1 script), Basic €9/mo, Plus €19/mo.

---

**15. Osano**

The Good: Industry-only $500K "No Fines, No Penalties" contractual guarantee covering regulatory fines if Osano is implemented per their guidance. Strong AI-assisted cookie classification with confidence scores users actually trust. Free tier for very small sites.

Frustrations: Self-serve cookie consent now starts at $199/month for a single domain capped at 30,000 visitors, substantially more than CookieYes / Termly. Banner customization repeatedly called out as limited.

Wish List: More customization. A mid-market tier between free and $199/mo.

Value for Money: 7/10. The guarantee is real value if you trust the implementation guidance.

Pricing: Free for very small sites, $199/mo for 30K visitors / 1 domain, enterprise custom.

---

**16. Termly**

The Good: Bundles legal policy generation (privacy policy, ToS, disclaimer) with the CMP. Useful one-stop for SMBs and freelancers. Aggressive entry pricing, Starter at $10/mo, Pro+ at $15/mo with 50K monthly banner views.

Frustrations: Free / Starter plan caps (1-2 policies, 10 edits, quarterly scans) push casual users to upgrade fast. Multi-platform users complain pricing scales awkwardly across multiple sites.

Wish List: A multi-site bundle.

Value for Money: 7/10. Strong SMB pick if you also need legal docs.

Pricing: Starter $10/mo, Pro+ $15/mo, multi-site custom.

---

**17. CookieYes**

The Good: Genuine free tier with 15K pageviews/mo, basic banner, one-domain auto-scan, enough for a small WordPress site to be GDPR-compliant for $0. Native WordPress plugin (formerly Cookie Law Info) with 1M+ active installs.

Frustrations: Per-domain pricing punishes multi-site operators. Agencies pay $10/mo Pro x N domains instead of one bundled fee. No DSAR automation, no API access, no policy generator on lower tiers.

Wish List: Agency / multi-site bundle.

Value for Money: 6.5/10. Solid free tier for one WP site. Wrong tool past that.

Pricing: Free 15K pageviews / 1 domain, Pro $10/mo per domain.

---

**18. CookieHub**

The Good: Session-based pricing instead of pageview metering. A single visitor browsing 30 pages still counts as 1 session, dramatically cheaper than Cookiebot for content-heavy sites. Genuinely useful free tier (1,000 sessions/mo, ~25K pageviews) with proof of consent and Google Consent Mode v2.

Frustrations: Syncing settings across multiple domains is reported as cumbersome. Limited features compared to OneTrust / Usercentrics tier, no A/B testing or advanced consent analytics.

Wish List: Multi-domain UX. Optional A/B module.

Value for Money: 7.5/10. Strongest pure-CMP value pick at the mid-market, especially for content sites.

Pricing: Free 1,000 sessions, paid tiers from low double digits monthly.

---

**19. ConsentManager (Iubenda-owned)**

The Good: Strong A/B testing + ML-driven banner optimization, vendor claims 15%+ avg consent rate lift. Live reporting with 12 dimensions and 30+ metrics, deepest analytics in the mid-market CMP segment.

Frustrations: Starts at €19 to €23/mo, pricier than CookieHub / CookieFirst at the same traffic tier. Bulk editing of new cookies and the auto-detected provider search reported as buggy.

Wish List: QA on the bulk-edit module.

Value for Money: 7/10. Right pick if you optimize banner consent rates seriously.

Pricing: From €19 to €23/mo.

---

## Tier 3: SMB / niche / discontinued

**20. Enzuzo**

The Good: Only CMP with a true Shopify-native integration that bundles policy generation, cookie consent, DSAR automation, multi-domain in the Shopify dashboard. Google Gold CMP Partner.

Frustrations: Free-tier privacy policy customization is limited. Lower-tier users report slow support escalation, no in-app way to contact the company.

Wish List: Tier-1 in-app support.

Value for Money: 7.5/10. The default Shopify CMP pick.

Pricing: Free tier with limits, paid tiers custom.

---

**21. Borlabs Cookie**

The Good: WordPress-native plugin with deep integration. Facebook Pixel assistant, content blockers, IAB TCF support, geo-restriction. Library of 350+ pre-built cookie / script packages.

Frustrations: WordPress-only, zero portability if you migrate to Shopify, Webflow, or headless. Once your annual subscription lapses, premium features (library, geo, IAB TCF, scanner, translations) stop working.

Wish List: Headless / framework-agnostic SDK.

Value for Money: 7/10. Strong WP pick. Painful when you grow off WP.

Pricing: Annual license, ~€39 to €99/yr depending on tier.

---

**22. Secure Privacy**

The Good: Coverage of 55+ global privacy laws (GDPR, CCPA / CPRA, LGPD, India's DPDP). Aggressive entry pricing ($8.33/mo) plus a free plan with Google Consent Mode v2 wired in.

Frustrations: Smaller brand than OneTrust / Didomi / Cookiebot, enterprise procurement often requires extra security questionnaires. Advanced reporting and customization gated to higher tiers.

Wish List: Brand recognition that matches the product.

Value for Money: 7/10.

Pricing: Free, paid from $8.33/mo.

---

**23. Privado**

The Good: Genuinely novel "privacy-as-code" approach, scans your codebase to auto-build data maps, RoPAs, PIAs, DPIAs without engineer interviews. AI agents (October 2025) for automating PIAs and data-mapping workflows.

Frustrations: Heavy false-positive rate in code scans, multiple G2 reviewers note review fatigue. Limited customization, slow scan performance on large monorepos. Not really a CMP-first product.

Wish List: Quieter, more accurate scans. CMP UX parity with the privacy-as-code engine.

Value for Money: 7/10 for engineering-led privacy ops. 5/10 if you only need a CMP.

Pricing: Custom.

---

**24. Quantcast Choice**

The Good: Was one of the only genuinely free TCF v2.0-compliant CMPs, adopted heavily by ad-supported publishers who couldn't justify paid CMPs. Implementation was famously simple, drop-in script.

Frustrations: Quantcast has discontinued the Choice CMP (as of late 2025), existing users must migrate. Limited customization vs paid CMPs always.

Wish List: Resurrection in some form. Honestly, just migrate.

Value for Money: N/A. Discontinued.

Pricing: Was free. No longer available.

---

## The first-party trust-infrastructure tier

This is the layer that asks the second question. Not just "is the consent banner certified," but "does my consent state live with my own data, and does it filter bots from the events I forward to ad platforms."

**25. DataCops**

The Good: TCF 2.2 certified first-party CMP. Consent state stored on your own subdomain (datacops.yourdomain.com), not pooled with the vendor. Customizable banner. Fraud-filtered consent signals (don't honor consent from bots) on the same pipeline that runs server-side CAPI to Meta + Google + TikTok + LinkedIn, plus first-party analytics, plus signup-fraud detection. White-label on the Talk-to-Sales tier. The bundle math: if you were going to buy a CMP at $30/mo + a CAPI gateway at $50/mo + a click-fraud tool at $59/mo + an analytics tool at $9/mo, this is the same job, one vendor, one DPA. IP reputation database publishes its size: 361B+ IPs and ranges, 146.4B+ datacenter, 11.9B+ VPN.

Frustrations: Newer than OneTrust, Didomi, Cookiebot. SOC 2 Type II is in progress, not active. The compliance page lists Google Consent Mode v2 as in progress. We don't carry the same regulatory-relationship pedigree as TrustArc (founded 1997 as TRUSTe). Smaller publisher network, so this is not the right pick if you're a Tier 1 EU publisher selling programmatic inventory.

Wish List: SOC 2 Type II completion. Google CMP Partner Gold tier (we're working through it). Native publisher-side SSP integrations.

Value for Money: 8.5/10 as a bundle for advertisers and SaaS sites. Not a like-for-like enterprise publisher CMP swap. Honest about both.

Pricing: Free tier is real (no card, 2,000 sessions/mo, free CMP, unlimited bot detection, 500 signup verifications). Growth $7.99/mo (5,000 sessions). Business $49/mo (50,000 sessions, HubSpot). Organization $299/mo (300,000 sessions). Enterprise talk-to-sales (single-tenant runtime, dedicated IP DB, custom DPA, EU/US residency, 99.9% uptime SLA, white-label CMP).

---

## So what should you actually use?

No true one-size-fits-all here. The real question is what you actually need.

- Tier 1 EU publisher selling programmatic inventory and you need TCF 2.3 with deep GVL / per-purpose vendor management? Sourcepoint (now Didomi), or Didomi directly. Or Sirdata if the data-share model fits.

- Enterprise privacy ops with multi-module needs (DSAR, RoPA, vendor risk, consent)? OneTrust if procurement requires the safe pick. TrustArc if you need the seal recognition. Securiti if the Veeam integration story fits. DataGrail if AI privacy ops matter.

- Mid-market with traffic and a need for soft session limits, no auto-upgrade billing? CookieHub, Ketch, or Iubenda.

- Shopify store? Enzuzo, full stop.

- WordPress single site? Borlabs Cookie if you stay on WP forever, CookieYes if you want a free tier, Termly if you also need legal policies bundled.

- Cookiebot user blindsided by the August 2025 pricing reset? CookieHub, Ketch, or DataCops on the bundle math.

- You only buy ads (not sell them) and someone tried to sell you TCF? You don't need TCF. You need Consent Mode v2. Pick any modern CMP that ships it (almost all of them in this list).

- You buy ads at scale, want consent + CAPI + bot filter + analytics on one bill, and your engineering team likes a real free tier for evaluation? DataCops.

- Need SOC 2 Type II on a signed letter today? OneTrust, TrustArc, Securiti. We have it in progress, not active.

---

## The mistake I see people make

Buying a TCF-certified CMP when they only buy ads. The CMP vendor's sales team sees the "TCF" question in the lead form and routes you to the publisher SKU. That SKU costs three to ten times the advertiser SKU and has features (GVL refresh cadence, per-purpose vendor management, disclosedVendors segment compliance) you'll never use. The decision tree at the top of this post is the single highest-ROI piece of advice in the category. Run it before talking to any CMP sales team.

---

## Now your turn

What triggered your CMP shopping in 2026? Cookiebot pricing reset? Didomi-Sourcepoint merger uncertainty? OneTrust enforcement? TCF 2.3 cutover? Drop the trigger and the size of the site, and I'll tell you which tier matches.

---

Research by [DataCops](https://www.joindatacops.com) · First-party tracking, consent infrastructure & fraud prevention.
