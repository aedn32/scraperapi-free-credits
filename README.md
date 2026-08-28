# ScraperAPI Free Credits: How to Get 5,000 Trial Credits + 1,000 Monthly Free Credits — Sign Up, Claim, and Stretch Every Credit (With Full Plan Pricing Breakdown)

If you've ever tried to scrape a website and watched your script get blocked, throttled, or fed a CAPTCHA wall, you already know why services like ScraperAPI exist. The harder question is the one most people actually type into Google: **how do the free credits work, how much can you really do with them, and is the free tier enough before you have to pull out a credit card?**

This is the part where most "reviews" wave a hand and say "1,000 free credits, great for testing!" — which is technically true and practically useless, because a single request to a Cloudflare-protected page with rendering turned on can burn 75 of those credits in one shot. So let's actually walk through what the free credits buy you, how to claim them, how to stretch them, and where the paid plans kick in once you've outgrown the free bucket.

## What ScraperAPI Free Credits Actually Are

ScraperAPI hands out free credits in two layers, and the distinction matters more than it sounds.

The first layer is the **permanent free plan**: 1,000 API credits every month, with up to 5 concurrent connections, no credit card required, and it renews automatically each month. This is the "always free" tier — you can keep using it indefinitely for small scraping jobs, monitoring a handful of pages, or running periodic checks.

The second layer is the **7-day free trial bonus**: when you first sign up, you get bumped up to 5,000 credits for the first seven days. This is a one-time boost on top of the free plan, designed to let you actually test the service against your real scraping targets (not a toy example) before you decide whether to pay for anything. After the 7 days expire, you drop back down to the 1,000-credit monthly free plan unless you upgrade.

> Note: unused credits do not roll over. Whatever you don't use resets at the end of each billing cycle, so there's no point stockpiling them.

## How to Claim Your Free Credits (Step by Step)

The signup process is genuinely simple — no credit card, no trial-then-charge trickery. Here's the flow:

1. **Head to the signup page** through the promotional link — 👉 [claim your 5,000 free trial credits here](https://www.scraperapi.com/?fp_ref=coupons). New accounts get the 5,000-credit trial automatically; no promo code is needed.
2. **Create an account** with your email (or Google/GitHub single sign-on). No payment information is requested at this stage.
3. **Grab your API key** from the dashboard. This is the single string you'll pass with every request.
4. **Test your first request** in the API Playground before scaling up — the Playground lets you preview results and see the exact credit cost per request for your specific target URLs.
5. **Use the Domain Multiplier tool** in the dashboard to look up the credit cost for any URL before you start scraping at scale. This is the single most important habit to build during your trial week.

If you need more than 5,000 credits for a serious evaluation (say, you're testing at production scale), the signup page notes you can contact support to claim up to 50 million scraping credits for proper speed and success-rate testing. That's a sales conversation, not a self-serve button, but it's there for teams doing due diligence.

## The Credit Math Nobody Explains Until It's Too Late

Here's the part that catches almost everyone off guard. The "1,000 free credits" and "5,000 trial credits" numbers sound generous until you understand that **one request does not equal one credit**.

The base rate is 1 credit for a standard, unprotected page. But the actual cost depends on the domain and the parameters you attach:

| Target / Parameter | Credit Cost per Request |
| --- | --- |
| Standard unprotected page | 1 |
| Amazon (e-commerce) | 5 |
| Google or Bing (SERP, all subdomains) | 25 |
| LinkedIn (social media) | 30 |
| Cloudflare / Datadome / PerimeterX bypass | +10 |
| `premium=true` parameter | +10 |
| `render=true` (JavaScript rendering) | +10 |
| `screenshot=true` | +10 |
| `ultra_premium=true` (paid plans only) | +30 |
| `premium=true` + `render=true` combined | 25 |
| `ultra_premium=true` + `render=true` combined | 75 |

So your 1,000 free monthly credits can mean:

- **1,000 plain requests** to unprotected blogs or news sites
- **200 requests** to Amazon product pages
- **40 requests** to Google search results
- **~33 requests** to LinkedIn pages
- **~13 requests** to a Cloudflare-protected site with ultra-premium proxy and rendering

This is why running your own numbers through the Domain Cost Estimator during the trial week is non-negotiable. The headline credit count tells you almost nothing without knowing your target mix.

One genuinely fair detail worth highlighting: **you're only billed for successful requests.** Failed scrapes (anything outside a 200 or 404 response) don't burn credits, so you're not paying for the service's own failures — only for data it actually delivered.

## How to Stretch Your Free Credits

If you're on the free plan or trial and want to squeeze maximum value out of every credit, a few habits make a real difference:

- **Use the API Playground first.** Before running any job at scale, test the target URL in the Playground to confirm it returns what you need and to see the exact credit cost.
- **Skip rendering when you don't need it.** JavaScript rendering adds 10 credits per request. If the data you want is in the static HTML, leave `render=false` and save 10x.
- **Avoid ultra-premium on the free tier.** The `ultra_premium=true` parameter (and the 75-credit ultra-premium + render combo) is only available on paid plans anyway, so this isn't an option on free — but it's worth knowing as you plan your upgrade path.
- **Cache aggressively.** If you're monitoring prices or listings that don't change every minute, store results locally and only re-scrape when something actually changes.
- **Stick to off-peak targets.** Sites with lighter anti-bot protection cost fewer credits. If you have flexibility in which sources you scrape, prioritize the cheaper ones during your trial.
- **Set credit spending limits.** The dashboard lets you cap your credit expenditure so a runaway script can't drain your entire monthly allowance in an afternoon.

## When the Free Credits Run Out: The Full Plan Lineup

Once you've outgrown the free tier — or once you need features like ultra-premium proxies, global geotargeting outside the US/EU, or pay-as-you-go overflow — the paid plans kick in. Here's the complete current lineup, pulled from the official pricing page, with every tier included so nothing is hidden.

| Plan | Monthly Price | Annual Price (10% off) | API Credits / Month | Concurrent Threads | Geotargeting | Purchase |
| --- | --- | --- | --- | --- | --- | --- |
| **Free** | $0 | — | 1,000 (renews monthly) | 5 | US & EU only | [Start free](https://www.scraperapi.com/?fp_ref=coupons) |
| **Free Trial (7 days)** | $0 | — | 5,000 (one-time) | 5 | US & EU only | [Claim 5,000 trial credits](https://www.scraperapi.com/?fp_ref=coupons) |
| **Hobby** | $49/mo | $44.10/mo | 100,000 | 20 | US & EU only | [Get the Hobby plan](https://www.scraperapi.com/?fp_ref=coupons) |
| **Startup** | $149/mo | $134.10/mo | 1,000,000 | 50 | US & EU only | [Get the Startup plan](https://www.scraperapi.com/?fp_ref=coupons) |
| **Business** | $299/mo | $269.10/mo | 3,000,000 | 100 | Global | [Get the Business plan](https://www.scraperapi.com/?fp_ref=coupons) |
| **Scaling** (most popular) | $475/mo | $427.50/mo | 5,000,000 | 200 | Global | [Get the Scaling plan](https://www.scraperapi.com/?fp_ref=coupons) |
| **Professional** | $975/mo | $877.50/mo | 10,500,000 | 300 | Global | [Get the Professional plan](https://www.scraperapi.com/?fp_ref=coupons) |
| **Advanced** | $1,975/mo | $1,777.50/mo | 21,500,000 | 500 | Global | [Get the Advanced plan](https://www.scraperapi.com/?fp_ref=coupons) |
| **Enterprise** | Custom | Custom | 22,000,000+ | 500+ | Global | [Contact sales for Enterprise](https://www.scraperapi.com/?fp_ref=coupons) |

A few things worth noting from this table that aren't obvious at a glance:

- **Geotargeting is gated by tier.** Free, Hobby, and Startup are limited to US & EU proxies only. If your project needs country-level targeting anywhere else in the world, you need at least the Business plan.
- **Pay-as-you-go overflow is only available from Scaling upward.** On Hobby, Startup, and Business, running out of credits mid-cycle means either upgrading to the next tier or talking to support — there's no PAYG overflow option.
- **Credits don't roll over.** Whatever you don't use resets at renewal, so it's worth sizing your plan to your actual monthly volume rather than overbuying "just in case."
- **Unlimited analytics history** kicks in starting at the Business plan; Hobby and Startup are capped at 30 days of dashboard history.
- **All paid plans include** JS rendering, premium proxies, JSON auto-parsing, rotating proxy pools, custom headers, CAPTCHA/anti-bot bypass, custom sessions, automatic retries, unlimited bandwidth, and a 99.9% uptime guarantee — the difference between tiers is volume, concurrency, and geotargeting scope.

## Which Plan Should You Actually Pick?

This is the question that matters more than the raw price tag, since the "right" plan depends entirely on what you're scraping and how often.

**Pick the Free plan if:** You're running a personal project, learning the API, or doing periodic small-scale monitoring. The 1,000 monthly credits cover a surprising amount of ground for plain unprotected pages.

**Pick Hobby ($49/mo) if:** You've outgrown the free tier but you're still in side-project or prototype territory — checking competitor prices on a handful of products, monitoring a few dozen pages, or building a proof of concept. 100,000 credits sounds like a lot until you remember Amazon costs 5x and Google costs 25x; for plain unprotected pages, though, this genuinely covers a lot of ground.

**Pick Startup ($149/mo) if:** You've outgrown casual scraping and need consistent volume — say, a small SaaS product or an agency running scraping jobs for a handful of clients. 1,000,000 credits with 50 concurrent threads is a meaningful step up, though you're still capped at US/EU geotargeting.

**Pick Business ($299/mo) if:** You need global geotargeting (not just US/EU), unlimited analytics history, or you're running production-grade infrastructure that other parts of your business depend on. This is also the first tier where the jump in concurrent threads (100) starts to matter for larger parallel jobs.

**Pick Scaling and above if:** You're past the "which plan" question and into "how do we keep this predictable at high volume" territory. These tiers add pay-as-you-go overflow billing so you're never hard-capped mid-month, plus priority support starting at Professional.

## What Happens If You Run Out of Credits Mid-Month?

This depends on which plan you're on:

- **Free, Hobby, Startup, Business (monthly):** You can seamlessly upgrade to the next plan tier, which usually provides a better price-per-credit. Or contact support to create a custom plan.
- **Hobby, Startup, Business, Professional (annual):** You can re-subscribe to start a fresh 12-month plan, or upgrade to a higher monthly plan that fits your new usage.
- **Scaling (monthly or annual), Professional, Advanced, Enterprise:** Pay-as-you-go kicks in — a pop-up lets you continue service using extra credits at a fixed, predictable rate. You can set a monthly spending cap so a runaway script doesn't surprise you with a huge bill.

Cancellation is available anytime from the dashboard, and there's a 7-day no-questions-asked refund policy if you're not satisfied.

## What People Actually Say About ScraperAPI

Independent review aggregation paints a fairly consistent picture: ScraperAPI sits around **4.5/5 on Trustpilot** and **4.4/5 on G2**, with the majority of reviews landing in five-star territory. The recurring praise points are the same across most platforms — clean documentation, a genuinely simple integration (drop it into existing code as a proxy replacement), and responsive support. One long-time reviewer specifically called out that upgrading or downgrading plans was painless, which tracks with how the credit system is structured.

On the critical side, the most common complaint isn't about reliability — it's about the credit math being less intuitive than the headline number suggests, especially once you start mixing in rendering and premium-proxy parameters on harder targets. Independent benchmarking from third-party testers has also noted that performance varies a lot by target: ScraperAPI tends to perform very well on mainstream sites like Amazon, GitHub, and standard e-commerce pages, but less consistently on sites with aggressive, frequently-changing anti-bot systems.

## How ScraperAPI Compares to Other Scraping APIs

If you're weighing this against alternatives, here's roughly how the positioning shakes out:

- **vs. Bright Data** — More powerful, more expensive enterprise option, generally starting around $499/mo, aimed at teams that need the highest possible success rates regardless of cost.
- **vs. Scrape.do** — Undercuts ScraperAPI on raw entry price (around $29/mo), which appeals to budget-conscious solo developers running simple, unprotected scrapes.
- **vs. ScrapingBee** — Similar developer experience and a comparable $49/mo entry point, generally without the same credit multiplier system, which makes its costs more predictable for some workloads.
- **vs. Oxylabs / ScrapingDog** — Strong alternatives if structured, platform-specific JSON output is your priority over raw HTML.

None of these are universally "better" — it depends on whether your priority is price predictability, raw success rate on hard targets, or ease of integration. For most developers running moderate-volume scrapes against mainstream sites, ScraperAPI's balance of price and simplicity is exactly why it remains one of the most recommended starting points in this category.

## Are There Any Active Discount Codes?

Beyond the 10% annual billing discount (which is automatic, no code needed), there are occasional promotional offers floating around coupon sites — but these change frequently and many are unverified. The most reliable way to lock in any current introductory offer is to sign up through the promotional link before subscribing, rather than hunting for coupon codes that may or may not actually work at checkout.

The cleanest deal that's always available: the **5,000-credit free trial with no credit card required**. That's the equivalent of getting paid-tier volume for a week to test your real workload before committing a single dollar. 👉 [Start your free trial here](https://www.scraperapi.com/?fp_ref=coupons).

## Frequently Asked Questions

**Does one API request always cost one credit?**
No. The base rate is 1 credit for a standard page, but the actual domain (Amazon, Google, LinkedIn, etc.) and any parameters you add (rendering, premium proxies) multiply that cost. Use the dashboard's Domain Multiplier to check before scraping at scale.

**What happens if I run out of credits mid-month?**
On Hobby, Startup, or Business, you can upgrade to the next tier (which usually comes with a better price-per-credit) or contact support about a custom arrangement. Scaling, Professional, Advanced, and Enterprise customers can keep scraping via pay-as-you-go at a fixed rate instead.

**Can I cancel anytime?**
Yes — cancellation is available anytime from the dashboard or by contacting support, and you won't be charged again after cancelling.

**Is there a refund policy?**
ScraperAPI offers a 7-day, no-questions-asked refund if you're not satisfied with the service.

**Do unused credits roll over?**
No. Your credit balance resets at each renewal, so it's worth matching your plan size to your actual monthly usage rather than stockpiling unused credits.

**Is the free plan really free forever?**
Yes. The 1,000-credit monthly plan is permanently free, no credit card required. The 5,000-credit trial is a one-time bonus on top of that, valid for the first 7 days after signup.

## The Bottom Line

If your scraping target is mostly plain pages without heavy anti-bot protection, the free plan's 1,000 monthly credits (plus the 5,000-credit trial week) genuinely covers a lot of ground for personal projects or early-stage prototypes. The moment Amazon, Google, LinkedIn, or Cloudflare-protected sites enter the picture, run your numbers through the credit table first — the sticker price and the real cost per successful scrape are two different things.

The cleanest way to find out which plan fits your actual workload is to just test it: sign up for the free trial, point it at your real targets, and watch your credit consumption in the dashboard before deciding anything. 👉 [Claim your 5,000 free trial credits and start testing now](https://www.scraperapi.com/?fp_ref=coupons).
