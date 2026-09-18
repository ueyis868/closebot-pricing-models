# ai sales agent pricing: per-message vs per-seat vs per-lead models, and the real monthly math behind CloseBot

Ask five vendors what an AI sales agent costs and you'll get five numbers that don't measure the same thing. One quotes $64 a month, another $9.99 per qualified lead, a third wants $900 a month for 1,200 messages. None of those figures is fake. They're just answers to different questions.

If you're trying to budget for an AI setter, the useful move isn't picking the lowest number off a pricing page. It's figuring out which billing model matches how your leads actually arrive, then working out the total monthly invoice — platform fee, usage, seats, storage, and whatever CRM sits underneath.

CloseBot is a good test case because it publishes one of the clearer pricing pages in this category, and because it sells two very different tracks (business and agency) off the same product. Here's how its numbers work, and how to compare them against everything else you'll be quoted.

## The three billing models you'll actually get quoted

Almost every AI sales agent on the market bills in one of three ways, or a hybrid of them.

**Per-seat** charges for each human who logs in. Instantly's 2026 pricing breakdown puts typical per-seat sales tools at $39–$109 per user per month, which worked fine when a license mapped to a human doing a fixed amount of work. It gets strange when one AI agent does the work of three setters — you end up paying for people, not output.

**Per-message (or per-credit)** charges for what the agent actually does. CloseBot's agency plan runs at $0.012 per message. HighLevel's published conversational AI rate, as summarized in CloseBot's own pricing comparison, is $0.02 per message pay-as-you-go. This model scales honestly with volume and can be brutal during a spike if you haven't set a ceiling.

**Per-outcome** charges only when something valuable happens. Fin for Sales, Intercom's inbound AI SDR, bills $9.99 per qualified lead. That's attractive when a qualified lead is worth thousands, and awkward when it isn't.

| Model | What you're billed for | Verified 2026 examples |
| --- | --- | --- |
| Per-seat | Each human user | $39–$109 per user/month (typical per-seat tools, per Instantly's breakdown) |
| Per-message / credit | Each AI reply or segment | CloseBot agency $0.012/message; HighLevel conversational AI $0.02/message |
| Per-outcome | Qualified lead, meeting, resolution | Fin for Sales $9.99 per qualified lead |
| Flat fee with a usage ceiling | Predictable base + included volume | CloseBot business plans from $64/month with 500 messages included; AiSDR from $900/month for 1,200 messages ($0.75/message) |

The flat-fee-with-ceiling model is the one most small teams end up wanting, because it caps the surprise. AiSDR's entry plan works out to roughly $0.75 per message at the included volume, which tells you something useful: on a pure per-message basis, that's a very different animal from $0.012.

## The costs that don't appear in the headline price

Budget the monthly subscription and you'll be short. Five lines show up later.

**Seats and storage.** CloseBot charges $5 per additional user per month on paid plans, and storage add-ons on business plans run $0.10 to $3.00 per MB per month depending on volume (1 MB of text is roughly 1,000 pages, so this is less scary than it sounds). On the agency plan, storage bills at $0.006 per MB per day and seats still cost $5.

**Overage.** The free plan includes 100 messages a month and then bills $0.08 per message. Business plans include 500 messages; go past your ceiling and you pay a 2x overage rate drawn from a prepaid wallet. Agency plans meter everything at $0.012.

**Model/token spend.** This is where vendors differ sharply. CloseBot doesn't let you plug in your own OpenAI or Anthropic key — the company calls it a security decision — so model access is bundled into what you pay. That's simpler than managing an API bill, and it means you can't shave costs by switching keys.

**The CRM underneath.** CloseBot is CRM-native: it takes over the text channels running through HighLevel, HubSpot, LeadConnector, or a custom CRM. Third-party pricing breakdowns put GoHighLevel at $97/month for Starter, $297 for Unlimited, and $497 for Agency Pro. If you already pay for a CRM, ignore this line. If you don't, it's part of your real cost. (CloseBot does list "standalone compatible" on its own comparison table, but the integrations the product is built around are CRM integrations.)

**Setup and supervision.** Template libraries and human support are included on paid CloseBot plans, but someone still has to configure the agent, test the flows, and watch the first few weeks of conversations. A quick scan of Reddit threads on CloseBot shows both sides of this: one agency owner in r/automation called it "way better than GHL chat AI"; another in r/gohighlevel said the learning curve put them off immediately. Build time is a real cost, not a footnote.

## Where CloseBot lands: the full plan line-up

Here's the current published structure, in one place. Prices are as listed on CloseBot's plans page.

| Plan | Who it's for | Key limits and inclusions | Price | Billing | Get it |
| --- | --- | --- | --- | --- | --- |
| Free | Testing the product, or very low lead volume | 100 messages/month, 1 MB storage, 1 user seat, 1 agent, unlimited account connections, unlimited custom field updates | $0 | Free forever under 100 messages; $0.08/message beyond | [ start on the CloseBot free plan](https://app.closebot.com/register?fpr=li87) |
| Core — Business | Businesses running their own pipeline | Message costs included in the base price, 500 messages/month, 15+ templates (50+ on annual), human support, add-on seats at $5 each, add-on storage and agents | From $64/month; $53/month equivalent when billed as $640/year | Monthly or annual | [ compare the business plans and message ceilings](https://app.closebot.com/settings?tab=subscription&plan=business&toggle=monthly&fpr=li87) |
| Core — Agency | Agencies building and reselling AI setters | Unlimited agents and sources, white-label client portal, rebill all costs, $0.012/message wholesale, seats at $5, storage at $0.006/MB/day | $397/month; third-party trackers list roughly $331/month on annual billing | Monthly or annual | [ open the agency plan details](https://app.closebot.com/settings?tab=subscription&plan=agency&toggle=monthly&fpr=li87) |
| Growth | Teams needing SLAs, compliance, or high volume | HIPAA compliance, quarterly audits, 99.99% priority uptime, priority support, 50+ templates | Custom quote | Custom | [ ask about the Growth plan](https://app.closebot.com/a?fpr=li87) |

A few details worth pulling out of that table.

The business plan slider runs from 100 messages a month up to 100K+, and the higher you raise the ceiling, the better the bulk rate. The published entry point is $64/month; third-party reviews that have tracked the slider put 1,000 messages around $84/month, 2,000 around $109, and 5,000 around $176. Treat those intermediate figures as third-party reporting rather than official pricing — CloseBot shows them dynamically, and pricing changes.

Annual billing gives you two months free across plans, plus the larger template library. On a $64/month plan that lands as $640 billed yearly, which is the $53/month figure you'll see on the page.

There's a 7-day trial of any paid plan before you're billed, plans run month to month with no lock-in, and CloseBot states plainly that there are no refunds. The trial is where you do your testing, not after.

One billing mechanic people miss: one message equals one segment, unless you switch on the Agent Node's "unlimited potential" (lots of tools, unlimited instruction size). That mode bills token costs instead, so a single message can consume several segments. If you plan to run heavy agents, budget above the base message count.

## The agency math is the interesting part

The agency plan exists for one reason: rebilling. You pay CloseBot $0.012 per message and can mark it up to whatever your client will bear. The same applies to seats ($5 each) and storage ($0.006 per MB per day). Wallet payments from your clients settle into your Stripe account through Stripe Connect; you top up your own wallet to cover the wholesale side.

CloseBot's own blog has published two worked examples from real accounts. The scaled one: 102 sub-accounts, about 108 conversational appointments a day, roughly 24,720 messages in a month, 50 MB of uploaded knowledge. That account pays $397 base + $148 in message costs + $9 storage + $255 in OpenAI tokens = $809/month. Switching the same account to DeepSeek models would have cut it to $617 — which is the clearest argument I've seen for why model choice matters more than plan tier once you're at volume.

The early-stage example: 4 sub-accounts, 468 messages, 3 MB of storage, DeepSeek. Total $403.50/month. If that same operator had used business plans instead, 500 messages a month are included for $64 with no per-message cost — which is the honest answer to "agency plan or business plan?" for anyone under roughly 500 messages a month who isn't reselling.

Those numbers come from CloseBot's own case studies, so read them as vendor-published illustrations, not audited benchmarks. But the arithmetic is transparent, which is more than you can say for most pricing pages in this category.

If you sell AI setting as a service, the rebilling layer is the one feature that turns a software bill into a revenue line. Most vendors in this space — including Fin and most per-seat tools — are direct-to-business products that don't support resale at all. That's a structural difference, not a feature-checklist difference.

## The number that actually decides this: cost per booked meeting

Platform fees don't matter much on their own. What matters is what you pay per appointment that lands on a calendar.

The arithmetic is `(platform + usage + storage + seats + CRM) / meetings booked`. Run it monthly, not annually — averaging over twelve months hides the bad months.

Put it next to the human alternative and the scale becomes obvious. Instantly's analysis, citing SalesHive, puts a fully loaded human SDR at $110,000–$160,000 in year one once you add benefits, payroll taxes, recruiting, and onboarding. A CloseBot business plan at $64/month with 500 included messages is $768 a year before CRM costs. Even the $809/month scaled example above lands at roughly $9,700 a year.

That's not a claim that AI setters replace sales teams, because they don't close anything — CloseBot qualifies, follows up, and books. But for the specific job of answering inbound leads within seconds at 11pm and remembering to follow up once, the cost comparison isn't close.

## Which plan fits which situation

A short, unsentimental version:

- **Under 100 messages a month, curious, no budget.** Stay on the free plan. It's free forever, it lets you build a real agent, and it includes unlimited custom field updates — a limit HighLevel's native AI only lifted to 20 fields recently.

- **500 to a few thousand messages a month, your own pipeline, no reselling.** Business plan. Message costs are included, which makes your invoice predictable in a way metered pricing never is. Pick the ceiling honestly; overages bill at 2x.

- **You sell AI setting to clients.** Agency plan, and check whether you're actually above the message volume where $0.012 wholesale plus your markup beats 500 included messages at $64. Below that volume, the agency plan is a $333/month premium for white-labeling and Stripe rebilling.

- **Healthcare, regulated industries, or you need SLAs and audits in writing.** Growth. It's a quote, and it's the only tier that lists HIPAA compliance, quarterly audits, and priority uptime.

- **Nothing to configure and nobody to configure it.** No plan fixes that. Every review I've read — positive or negative — lands on the same point: the conversation quality tracks the effort you put into the agent, and one G2 reviewer put it bluntly: sloppy follow-up logic just gets scaled faster.

## FAQ

**Does CloseBot charge extra per message on business plans?**

No — message costs are included in the base price up to your ceiling. Above the ceiling you pay a 2x overage rate from your wallet. Agency plans bill everything at $0.012 per message.

**Is there a free trial?**

Two things, actually. A free-forever plan capped at 100 messages a month, and a 7-day trial on any paid plan before billing starts. CloseBot states there are no refunds after that, so use the trial.

**Can I bring my own OpenAI or Claude API key to reduce costs?**

No. CloseBot explicitly disallows bring-your-own-key and describes it as a security decision. Model access is bundled.

**Does it work without a CRM?**

The site lists standalone compatibility, and it natively integrates HighLevel, HubSpot, LeadConnector, and custom CRMs. In practice, if your leads live somewhere, that "somewhere" is what CloseBot reads — so most setups pair it with a CRM you already pay for.

**Is CloseBot any good, or is this just cheap?**

It's not the cheapest per-message option and it isn't trying to be. On G2 it holds a 4.8/5 rating across 124 reviews, and CloseBot claims over 1 million booked appointments and 1,000+ agencies on the platform — vendor numbers, so weigh them accordingly. The recurring complaint is configuration effort, not conversation quality.

---

If there's one thing to take from all of this, it's that AI sales agent pricing in 2026 comes down to three questions: does the vendor bill by human, by message, or by result; what happens when you blow past your ceiling; and can you pass any of it to a client. CloseBot picks its answers — flat base with included messages on business, metered and rebillable on agency — and publishes the overage rules rather than hiding them in a sales call.

[👉 Check the current CloseBot plans and start on the free tier](https://app.closebot.com/a?fpr=li87) before you commit to anything, and run your own cost-per-meeting math against your actual lead volume. That number will tell you more than any pricing page.
