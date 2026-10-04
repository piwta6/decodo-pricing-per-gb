# decodo pricing: What Every Tier Costs Per GB, and When a Per-IP Plan Comes Out Cheaper

Search "decodo pricing" and the first number you meet is "from $2 per GB." Scroll to the plan cards on the same page and the cheapest one reads $3.75 per GB. Pay-as-you-go is $4.00. All three figures are real, which is why this particular shopping trip takes longer than it should.

Decodo is the company formerly known as Smartproxy (the footer still says so). It sells residential, mobile and datacenter proxies plus a few scraping products, and each of those lines has its own pricing logic. Below is the full picture: every self-serve tier, what sits behind the enterprise tab, what the trial and refund rules actually cover, and the one billing model Decodo doesn't offer — per-IP with unlimited traffic — which changes the math for a specific kind of workload.

## Decodo pricing at a glance

Different products, different units, so a single price is meaningless without a label:

- Residential proxies: from $2 per GB at the highest volumes; the cheapest self-serve card is **$3.75 per GB**
- Mobile proxies: from $2.25 per GB
- Datacenter proxies: from $0.020 per IP
- Web Scraping API: from $0.09 per 1,000 requests
- Video Downloader: from $0.08 per GB
- AI Parser and MCP server: free
- Fast Search API: price on request

Residential is the line most people are here for, so start there.

## Residential proxy tiers, tier by tier

| Plan | Rate per GB | Monthly price (excl. VAT) |
| --- | --- | --- |
| 3 GB | $3.75 | $11.25 |
| 10 GB | $3.50 | $35 |
| 25 GB (Decodo's "popular" tier) | $3.25 | $81.25 |
| 50 GB | $3.00 | $150 |
| 100 GB | $2.75 | $275 |
| Pay as you go | $4.00 | No commitment |
| Enterprise 250 GB | $2.50 | $625 |
| Enterprise 500 GB | $2.25 | $1,125 |
| Enterprise 1 TB (1,000 GB) | $2.00 | $2,000 |

Two things about that table matter more than the numbers. First, the enterprise rows live on a separate tab and aren't part of the normal checkout flow. Second, every rate drops as volume rises — there's no volume tier where you pay more per gigabyte than you would buying a single gigabyte at a time.

Decodo's residential page carries a "last updated" stamp and lists these figures excluding VAT, billed monthly. The plan includes city, ZIP code and ASN targeting at no extra charge, across 195+ locations and a pool the company sizes at 115M+ residential IPs. That matters because granular targeting is one of the few features competitors reliably charge extra for.

## Why "from $2/GB" and $3.75/GB are both correct

The $2 headline is the 1 TB enterprise rate. It's an honest number, it's just not the number most buyers will pay. Comparison sites that flagged the gap are right to flag it: the cheapest card a self-serve customer can click is $3.75 per GB on the 3 GB plan, and pay-as-you-go is $4.00.

There's a second quirk worth knowing before you commit. On subscription plans the monthly allowance is use-it-or-lose-it: bandwidth doesn't carry into next month, so a 25 GB plan where you burn 9 GB most months is effectively a $81.25 purchase of 9 GB. Third-party comparisons point this out, and it's the kind of detail that quietly doubles someone's effective per-GB cost. If your traffic is spiky rather than steady, check whether the cheapest tier you'll actually finish is a smaller plan, or whether per-GB validity matters more to you than headline rate.

## Mobile, datacenter and scraping products

Residential isn't the whole catalog, and the other lines have their own starting rates:

| Product | Entry price | Notes |
| --- | --- | --- |
| Mobile proxies | from $2.25 per GB | 10M+ mobile IPs, 700+ carriers, 160+ locations |
| Datacenter proxies | from $0.020 per IP | Priced per IP; scales with how many you rent |
| Web Scraping API | from $0.09 per 1,000 requests | Subscription tiers run free → $19 → $49 → $99 per month, with rate limits stepping up from 10 to 50 requests per second |
| Video Downloader | from $0.08 per GB | Per-GB bandwidth pricing |
| Fast Search API | On request | Quote-based |
| AI Parser | Free | Turns page HTML into structured JSON |
| MCP server | Free | Lets AI agents and tools browse through Decodo |

Mobile is billed on traffic like residential, so the same volume logic applies: $2.25 per GB is a large-commitment rate, not the entry rate.

## What comes with a paid plan

Worth reading before you decide the pricing is too high or too low:

- **Free trial:** 100 MB over three days, activated after card verification. It's a genuine trial, not a demo dashboard.
- **Refunds:** 14 days, but conditional. The policy covers self-service purchases, excludes crypto payments, excludes purchases made during a free trial, applies only to your first purchase of a given service, and requires that you've used less than 20% of the plan quota or 1 GB, whichever comes first.
- **Targeting:** continent, country, state, city, ZIP and ASN, included in the plan price.
- **Payment methods:** cards through Stripe and Cleverbridge, plus crypto through CoinPayments.
- **Session control:** rotating sessions, sticky presets of 1, 10, 30 or 60 minutes, and a custom duration.

> The refund window and the free trial don't overlap. Signing up for the trial and then buying removes your refund eligibility on that purchase — a detail buried in the conditions, not in the marketing copy.

## How Decodo's pricing holds up in independent testing

AIMultiple's 2026 proxy pricing benchmark measured GB-per-dollar from 10 GB to 10 TB and ranked Decodo first on residential cost-efficiency, ahead of Oxylabs, Bright Data and Apify. A separate low-volume comparison from the same researchers found Decodo had the lowest total residential price at every tested point between 10 GB and 200 GB. PCMag's head-to-head against IPRoyal reached a similar conclusion in softer language: affordable, easy-to-follow plans that suit small businesses.

Not everyone agrees. CNET gave Decodo a middling value score and called its bulk data packages expensive. Read the CNET table closely, though, and you'll see 2 GB for $6.00 and 8 GB for $5.50 — tiers that no longer exist at those prices. Reviews with hardcoded price tables age badly in this market, which is the practical reason to check the live page rather than the review.

## The billing model Decodo doesn't sell

Every Decodo product is billed by volume: gigabytes for residential and mobile, IPs per month for datacenter, requests for the API. If you want a fixed number of residential IPs with unlimited bandwidth and no expiry, there's no plan for it.

9Proxy builds its residential business around exactly that model, plus a per-GB option for rotation-heavy work. The two products are structured differently on purpose:

- **Residential by IPs** — you pay per IP, traffic through it is unlimited, and unused IPs never expire. Each IP stays alive somewhere between a few hours and about 24 hours. Setup requires the 9Proxy desktop app for local port forwarding.
- **Residential by GB** — you pay per gigabyte, generate unlimited endpoints, and get rotating or sticky sessions with 180-day validity on the balance (no expiry at all on enterprise GB packages). This one works straight from the dashboard, with username/password or IP whitelist authentication.

The pool is 20M+ residential IPs across 90+ countries, with country, city, ZIP and ISP targeting, HTTP/HTTPS and SOCKS5 support, and 24/7 support. Published entry rates are $0.015 per IP and $0.68 per GB at the top-volume tiers. IP-based and bundle packages went through a price adjustment on 1 June 2026 — the first in the company's history, per its own announcement — while GB-based pricing stayed put.

If a per-IP structure is the part that was missing from your Decodo comparison, 👉 [see the current 9Proxy packages and rates here](https://bit.ly/9-Proxy).

## 9Proxy pricing: the complete package list

Prices below reflect the post-June-2026 IP and bundle rates. The "$0.015 per IP" and "$0.68 per GB" figures you'll see advertised are top-tier rates, not entry rates — same caveat as Decodo's $2 headline.

| Package | Model | What you get | Price | Link |
| --- | --- | --- | --- | --- |
| 100 IPs | Per IP | 100 residential IPs, unlimited bandwidth, no expiry | $24 ($0.24/IP) | [check this package](https://bit.ly/9-Proxy) |
| 500 IPs | Per IP | 500 residential IPs, unlimited bandwidth | $72 | [current price](https://bit.ly/9-Proxy) |
| 1,000 + 500 IPs | Per IP | 1,500 IPs with bonus, unlimited bandwidth | $126 | [current price](https://bit.ly/9-Proxy) |
| 2,500 IPs | Per IP | Unlimited bandwidth per IP | $210 | [current price](https://bit.ly/9-Proxy) |
| 5,000 IPs | Per IP | Unlimited bandwidth per IP | $360 | [current price](https://bit.ly/9-Proxy) |
| 15,000 IPs | Per IP | Unlimited bandwidth per IP | $720 | [current price](https://bit.ly/9-Proxy) |
| 25,000 IPs | Per IP | Volume rate | ~$863 | [current price](https://bit.ly/9-Proxy) |
| 50,000 IPs | Per IP | Volume rate | ~$1,438 | [current price](https://bit.ly/9-Proxy) |
| 100,000 IPs | Per IP | Business tier | $2,300 | [current price](https://bit.ly/9-Proxy) |
| 200,000 IPs | Per IP | Business tier | $4,140 | [current price](https://bit.ly/9-Proxy) |
| 500,000 IPs | Per IP | Business tier | $8,625 | [current price](https://bit.ly/9-Proxy) |
| 5 GB | Per GB | Rotating or sticky, 180-day validity | $15 ($3.00/GB) | [check this package](https://bit.ly/9-Proxy) |
| 50 + 5 GB | Per GB | Bonus bandwidth, 180-day validity | $105 ($2.10/GB) | [current price](https://bit.ly/9-Proxy) |
| 100 GB | Per GB | 180-day validity | $150 ($1.50/GB) | [current price](https://bit.ly/9-Proxy) |
| 200 GB | Per GB | 180-day validity | $200 ($1.00/GB) | [current price](https://bit.ly/9-Proxy) |
| 1,000 GB | Per GB | 180-day validity | $800 ($0.80/GB) | [current price](https://bit.ly/9-Proxy) |
| 2,000 GB | Per GB | 180-day validity | $1,500 ($0.75/GB) | [current price](https://bit.ly/9-Proxy) |
| 3,000 GB (Enterprise) | Per GB | No expiry | $2,160 ($0.72/GB) | [current price](https://bit.ly/9-Proxy) |
| 6,000 GB (Enterprise) | Per GB | No expiry | $4,200 ($0.70/GB) | [current price](https://bit.ly/9-Proxy) |
| 10,000 GB (Enterprise) | Per GB | No expiry | $6,800 ($0.68/GB) | [current price](https://bit.ly/9-Proxy) |
| 100 IPs + 5 GB | Bundle | Starter combination | $30 | [grab the starter bundle](https://bit.ly/9-Proxy) |
| 1,500 IPs + 50 GB | Bundle | Mid-volume combination | $180 | [current price](https://bit.ly/9-Proxy) |
| 5,000 IPs + 500 GB | Bundle | High-volume combination | $720 | [current price](https://bit.ly/9-Proxy) |

Two structural notes. The balance-based system means nothing renews automatically — you buy a package, and IP-based packages keep their IPs until they're used. And the IP-based model's desktop-app requirement is a real constraint, not fine print: if you need proxies that integrate into a server-side pipeline with nothing installed locally, the GB-based model is the one that fits.

## The math: 100 GB on Decodo vs 9Proxy by the IP

Take a workload that moves 100 GB a month. On Decodo's residential plans that's **$275 per month, resetting to zero each cycle**. On 9Proxy's GB model, 100 GB is $150 with a 180-day window to use it — half the monthly outlay, and the balance doesn't evaporate on the 30th.

Now change the assumption. Suppose your actual usage is 100 long-lived sessions pushing heavy traffic: account work, dashboards, price monitoring in a couple of markets. Decodo bills the traffic, so 100 GB still costs $275. A 9Proxy package of 100 IPs costs $24 with unlimited bandwidth per IP. Same nominal bandwidth, roughly a tenth of the spend — provided you can live with IPs that last hours rather than persist for months, and with the desktop app.

Where Decodo keeps the edge: a smaller number of requests spread across a much wider rotation, ZIP and ASN-level targeting, a larger residential pool, and native integration with its own scraping API and unblocker under one dashboard. That's a workflow question, not a price question.

## Which one to buy

- **Steady, predictable traffic and you want one vendor for proxies plus scraping:** Decodo's 10 GB or 25 GB tier is the sensible start, at $35 or $81.25 plus VAT.
- **Bandwidth-light but rotation-heavy — millions of small requests:** GB billing wins on both. 9Proxy's 100 GB at $150 with 180-day validity is cheaper than Decodo's monthly 100 GB, and the balance survives a slow month.
- **Bandwidth-heavy through a fixed set of sessions:** per-IP is the outlier worth testing. $24 for 100 IPs with unlimited traffic isn't a rate Decodo's model can match, because Decodo's model doesn't bill that way.
- **You need ZIP or ASN targeting built into the plan price:** Decodo includes it; 9Proxy includes country, city, ZIP and ISP targeting on its side. Neither charges extra, so this isn't the deciding factor.

If the per-IP route is the one that matches your workload, 👉 [start from the 9Proxy signup page](https://bit.ly/9-Proxy) and size the package against your session count rather than your gigabyte estimate.

## FAQ

**Does unused bandwidth roll over?**
On Decodo's residential subscriptions, no — the monthly allowance resets. On 9Proxy's GB packages you get 180 days to use the balance, and enterprise GB packages don't expire at all.

**Is there a free trial?**
Decodo gives 100 MB over three days, activated after card verification, and that trial purchase is excluded from the 14-day refund policy. 9Proxy lists a free trial too; confirm eligibility at signup, since trials in this market are usually gated behind a sales or support conversation.

**Can I pay monthly instead of committing?**
Decodo's plans are monthly with auto-renew, and pay-as-you-go at $4.00 per GB is available if you don't want a recurring charge. 9Proxy doesn't run subscriptions — packages are purchased from a balance, and IP-based packages keep their IPs until used.

**Do these prices include tax?**
No. Decodo lists rates excluding VAT, with the final amount depending on your country. Decodo accepts cards through Stripe and Cleverbridge, plus crypto through CoinPayments.

**What's the cheapest way to actually test a provider?**
On Decodo, the 3 GB plan at $11.25 is the smallest paid tier, though the 100 MB trial costs nothing. On 9Proxy, the 100-IP package at $24 is the lowest entry point that comes with unlimited traffic per IP, and the unused IPs stay in your account indefinitely.

Prices in this market move — Decodo's page carries a revision date, and 9Proxy changed its IP and bundle rates on 1 June 2026 while leaving GB pricing alone. Treat the tables above as a starting map and confirm the current figures at checkout before you commit budget to either one.
