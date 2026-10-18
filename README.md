# dedicated server hosting uk: real prices compared, and when Vultr's hourly-billed London bare metal beats a fixed monthly contract

UK dedicated server sellers fall into two camps. Local specialists such as EUGameHost and Hosting UK run their own British data centres and want you on a monthly contract, starting at £45–£69. Vultr works differently: London is one of its 30-plus global locations, bare metal is billed by the hour with no setup fee, and new accounts get up to $250 in credit to spend within 30 days.

Neither model is automatically cheaper. If you need a server for a year and want engineers on site, the UK specialists make sense. If the project might end in six weeks, or you're still sizing hardware, paying for exactly the hours you use changes the maths completely. Below: the real listed prices from the main UK players, Vultr's bare metal line-up in full, and the small print that decides your first-year bill.

> **Quick picks**
>
> - Full physical server in London, zero commitment: Vultr bare metal from **$120/month**, hourly billing, no setup fee. 👉 [check the bare metal line-up and London stock](https://www.vultr.com/products/bare-metal/?ref=7268283)
> - Game servers with game-layer DDoS filtering: EUGameHost, from £45/month, own UK data centre.
> - Managed support, Windows, 100% uptime SLA: Hosting UK, from £69/month.
> - 32-core EPYC muscle and guaranteed traffic: Leaseweb (AMD from £123) or HOSTKEY (EPYC 9354 configs from €307).

## What dedicated servers in the UK actually cost right now

Entry-level UK dedicated servers sit between £45 and £99 a month. Mid-range boxes with 8-plus cores land around £85–£160, and serious EPYC or dual-Xeon hardware runs from roughly €238 up to £500. Five providers cover most of the market, and their entry listings look like this:

| Provider | Cheapest listed plan | What that buys | Watch-outs |
| --- | --- | --- | --- |
| EUGameHost | £45/mo, Intel i7-6700 | 4c/8t, 32GB RAM, 500GB NVMe, 10Gbps port, 30Tbps game-aware DDoS, own UK data centre | Game-focused; free setup |
| Hosting UK | £69/mo, Xeon E3-1270v5 | 64GB RAM, 4x250GB SSD, unlimited bandwidth, Dell hardware | Managed options cost more; flagship dual Gold configs reach £499 |
| OVHcloud UK | £98.99 ex VAT/mo, Advance-1 | EPYC 4244P 6c/12t, 32–192GB, NVMe, 1–5Gbps, anti-DDoS included | £98.99 ex VAT setup fee on entry plans |
| Leaseweb UK | £64/mo, High Bandwidth | High Performance from £77.59, Gaming from £79.73, AMD servers from £123 | Outgoing traffic depends on the traffic plan you pick |
| HOSTKEY | from €238/mo | Dual Gold 6140 with 256GB RAM; EPYC 9354 32-core systems from €307 with up to 10Gbps | Unmanaged; administration is a paid extra |

All five host on monthly terms. Keep that in mind for the next section, because it's where Vultr's model diverges.

## Vultr's version of a dedicated server: bare metal, plus a cheaper middle ground

Bare metal at Vultr means a whole physical machine with full root access, provisioned through the same panel and API as its cloud VMs. Billing is hourly and capped at the monthly rate, so a server you destroy after three weeks costs about three-quarters of the monthly price. If a full chassis is more than you need, Vultr's Optimized Cloud Compute range offers dedicated vCPUs (cores no other tenant can schedule onto) from $28/month, which covers most "I just want reserved CPU" cases at a fraction of bare metal cost.

The bare metal line-up:

| Plan | CPU | RAM | Storage | Monthly price | Deploy |
| --- | --- | --- | --- | --- | --- |
| E3-1270v6 | 4c/8t @ 3.8GHz | 64GB DDR4 | 2x240GB SSD | $120 | [Deploy E3-1270v6](https://www.vultr.com/products/bare-metal/?ref=7268283) |
| E5-2650 v4 | 12c/24t @ 2.2GHz | 128GB DDR4 | 2x480GB SSD | $185 | [Deploy E5-2650 v4](https://www.vultr.com/products/bare-metal/?ref=7268283) |
| Dual E5-2690 v4 | 28c/56t @ 2.6GHz | 256GB DDR4 | 2x480GB SSD | $325 | [Deploy Dual E5-2690 v4](https://www.vultr.com/products/bare-metal/?ref=7268283) |
| EPYC 7302P | 16c/32t @ 3.0GHz | 128GB DDR4 | 2x960GB NVMe | $370 | [Deploy EPYC 7302P](https://www.vultr.com/products/bare-metal/?ref=7268283) |
| EPYC 7402P | 24c/48t @ 2.8GHz | 256GB DDR4 | 2x1.92TB NVMe | $495 | [Deploy EPYC 7402P](https://www.vultr.com/products/bare-metal/?ref=7268283) |
| EPYC 7502P | 32c/64t @ 2.5GHz | 256GB DDR4 | 2x3.84TB NVMe | $650 | [Deploy EPYC 7502P](https://www.vultr.com/products/bare-metal/?ref=7268283) |

All monthly prices include hourly billing and no setup fee; larger dual-socket systems sit above this range.

Two caveats worth knowing before you plan anything around these numbers. Vultr rotates its chassis over time as newer CPU generations arrive, so the exact models on offer shift. And stock varies by region, so the deploy screen is the only reliable way to confirm which plans are live in London on a given day.

For completeness: Vultr also sells shared Cloud Compute from $5/month (fine for staging sites, nowhere near a dedicated server), High Frequency instances from $6/month, GPU servers, and managed databases. Those exist for other workloads; the two options above are the ones relevant to a dedicated server search.

## The billing details that decide whether Vultr saves you money

Vultr wins on time flexibility and the absence of setup fees, and it can lose on traffic guarantees and DDoS, which are extras rather than standard. Five specifics:

1. **Setup fees.** OVHcloud's Advance-1 costs £118.79 including VAT per month, plus £98.99 ex VAT to install. Month one effectively doubles. Vultr charges nothing to provision, and destroying a server stops the meter the same hour.
2. **The $250 credit.** New signups get up to $250 usable within 30 days of activation (you'll need to add a payment method first). That's enough to run the $120 E3-class box for two months before paying anything, which makes it a genuine proof-of-concept budget. None of the five UK specialists above offers anything comparable on their listed pages. 👉 [claim the credit and run your own numbers](https://www.vultr.com/pricing/?ref=7268283)
3. **Currency.** Vultr bills in US dollars, so its prices don't map one-to-one against the pound figures elsewhere in this piece. Your card issuer handles conversion, and checkout applies tax based on your billing address.
4. **DDoS.** OVHcloud includes anti-DDoS protection as standard, and EUGameHost filters 30Tbps of game-specific traffic. Vultr sells DDoS protection as an optional $10/month add-on per server. For anything public-facing, price that in from the start.
5. **Traffic.** HOSTKEY and Leaseweb publish concrete traffic allowances (50TB and up on many configs). If guaranteed outbound transfer matters to your project, compare each Vultr plan's allowance directly against those bundles before deciding.

## Where the UK specialists still beat Vultr

Three groups of buyers should look elsewhere, and it's better to say so upfront.

If you want someone else to handle the server, Hosting UK is the stronger fit. Its engineers work from its own data centres 24/7, managed packages are available on every server, Windows Server 2022/2019 and SQL Server licences are on the menu, and the company publishes a 100% uptime guarantee backed by an SLA. Vultr is self-service by design: tickets get answered around the clock, but nobody will patch or tune your machine for you.

Game server communities have a purpose-built option in EUGameHost. Its entry plans run overclocked cores up to 6GHz, cache A2S queries at the edge for faster server browsing, and apply game-aware filtering across a 30Tbps DDoS network, all from its own UK facility. A generalist bare metal box can host games, but it won't match that stack for Minecraft, Rust, ARK, CS2 or FiveM populations.

Heavy workloads with contractual teeth belong with the big outfits. HOSTKEY's EPYC 9354 systems scale up to 768GB of DDR5, and Leaseweb pairs its UK servers with an ISO-certified data centre footprint and a 99.999% core network uptime claim. A $120–$650 single-socket range doesn't compete in that weight class, and it isn't trying to.

Where Vultr does fit: agencies spinning up short-lived client environments, developers who need disposable physical hardware for a sprint, teams validating a workload before committing to a contract, and anyone whose project length is genuinely unpredictable. If that describes you, 👉 [browse Vultr's current bare metal configurations](https://www.vultr.com/products/bare-metal/?ref=7268283) and check London stock first.

## Deploying a Vultr bare metal server in London

The whole process happens in the control panel and takes minutes of actual work.

1. **Create an account and add a payment method.** This is what activates the trial credit, so don't skip it.
2. **Pick a plan and region.** Under Bare Metal, choose your chassis and select London. If your preferred plan shows no UK stock, the deploy screen tells you which regions have it.
3. **Choose the OS.** Standard Linux images install automatically; for a specific build, mount your own ISO during setup.
4. **Add extras, then deploy.** A DDoS-protected IP costs $10/month if you're running something public-facing. Once deployed, the server appears in your panel, billing runs by the hour, and you can reinstall or rescue it without raising a ticket.

👉 [open the bare metal deploy page](https://www.vultr.com/products/bare-metal/?ref=7268283) and the availability check takes about thirty seconds.

## FAQ

**Does Vultr have a UK data centre?**
Yes. London is one of Vultr's 30-plus cloud locations, and it serves both cloud compute and bare metal. Chassis availability varies by region, so confirm your specific plan is stocked in London before migrating.

**How much does a dedicated server in the UK cost?**
Entry plans run £45–£99 per month, mid-range 8-core-plus machines £85–£160, and premium EPYC or dual-Xeon systems £250 and up. Vultr's bare metal starts at $120/month with no setup fee and hourly billing.

**Is bare metal the same as a dedicated server?**
Yes. Bare metal is the cloud-industry term for a full physical machine leased to a single tenant, as opposed to a virtual server sharing hardware with other customers.

**Does Vultr include DDoS protection?**
DDoS protection is a paid add-on at $10/month per server. That contrasts with OVHcloud, which includes anti-DDoS as standard, and EUGameHost, which specialises in game-layer filtering.

**Can I run Windows on Vultr bare metal?**
Windows Server images are available on Vultr's cloud compute plans for a monthly licence fee. On bare metal, the usual route is mounting your own ISO with your own licence during setup.

**Can I cancel whenever I want?**
Yes. Vultr bills hourly and caps at the monthly rate, so destroying a server stops charges immediately. HOSTKEY offers something similar on its instant servers, crediting unused funds to your account balance.

## Before you order

Match the purchase to the shape of your workload. A predictable, year-long deployment that you'd rather not administer yourself points to Hosting UK's managed tiers. A game community with DDoS worries points to EUGameHost. Large EPYC builds with traffic guarantees point to HOSTKEY or Leaseweb. Anything short-term, spiky, or still being sized is where Vultr's hourly model pays off.

Three things to confirm before clicking order, whichever way you go: the chosen chassis is actually stocked in London, DDoS protection is sorted if the service is public-facing, and for Vultr specifically, that you've activated the credit within its 30-day window so the trial actually covers your test period. 👉 [create your Vultr account and deploy in London](https://bit.ly/VulTR)
