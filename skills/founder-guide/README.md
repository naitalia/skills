# Founder Guide

**English** · [中文](README.zh.md)

An open skill that gives AI assistants and agents twelve situation-based playbooks for the
decisions founders actually get stuck on — from "is anyone really going to pay for this?" to
"do I fire this executive?" to "the company may not make it to next quarter".

It is not a list of startup tips. Each playbook is built for one kind of situation and
answers it in a fixed shape:

- **Ask these first** — the questions that decide which advice applies to you
- **Plays** — concrete steps, each with what "done" looks like
- **Common traps** — how founders usually get it wrong
- **Two schools of thought** — where experienced people disagree, and the conditions for choosing
- **When this doesn't work** — the boundaries
- **How solid is the evidence** — whether a claim rests on broad observation, one experiment,
  or one practitioner's experience, and what later research weakened
- **Not covered** — what the playbook honestly cannot answer

## The twelve playbooks

| # | Playbook | Use it when… |
|---|---|---|
| 1 | [Direction and Demand Validation](playbooks/en/01-demand-validation.md) | I have an idea and friends and family all say it's great, but I'm not sure anyone would actually pay |
| 2 | [MVP and Product Trade-offs](playbooks/en/02-mvp-and-scope.md) | The product has been in the works for months and I keep feeling a few more features are needed before it's presentable |
| 3 | [Pricing](playbooks/en/03-pricing.md) | I'm setting the first price for a new product and customers have nothing to compare it with |
| 4 | [Early Acquisition and Growth](playbooks/en/04-early-growth.md) | I have no ad budget and don't know where my first users will come from |
| 5 | [Selling Big Deals to Businesses](playbooks/en/05-b2b-sales.md) | A customer said "very interested, let us think it over" and then went silent |
| 6 | [Positioning Against Stronger Competitors](playbooks/en/06-positioning-vs-incumbents.md) | A company with far more resources than us is about to enter our space, and the team is starting to panic |
| 7 | [Equity and Co-founders](playbooks/en/07-equity-and-cofounders.md) | My co-founder and I want to split the equity evenly, or within a point or two of it, and I don't know whether that's a hidden risk |
| 8 | [Hiring, Firing and Performance Reviews](playbooks/en/08-hiring-firing-reviews.md) | I have an hour to interview someone, the candidate answers every question smoothly, and I can't tell how they'll actually do on the job |
| 9 | [Managing the Team](playbooks/en/09-managing-the-team.md) | The team has grown from a dozen people to a few dozen, I'm busy from morning to night, and I can't say which of it actually matters |
| 10 | [Negotiation](playbooks/en/10-negotiation.md) | I'm about to negotiate terms with a customer, platform or investor far bigger than me, and it feels like they call the shots |
| 11 | [Judging Claims, Numbers and Forecasts](playbooks/en/11-judging-claims-and-forecasts.md) | I have an industry report with a gorgeous market size and growth rate, and I can't tell how far to trust it |
| 12 | [Crisis and Hard Decisions](playbooks/en/12-crisis-decisions.md) | The company may not survive, I lie awake asking what happens if it goes under, and I can't see the next step |

Every playbook exists in Chinese and English. The assistant answers in whatever language you
write in.

## Install

The skill is plain Markdown, so it works with any assistant that can read files. This folder —
`skills/founder-guide/` in the repository — is the whole skill.

To get it, open the repository's main page, click the green **Code** button → **Download ZIP**,
and unzip it.

**Agents with skill support.** Copy the `skills/founder-guide/` folder into the directory your
agent loads skills from, keeping the folder name `founder-guide`. The agent reads `SKILL.md`
first and opens the matching playbook only when your situation calls for it.

**Chat apps without skill support.** Paste the contents of this folder's `SKILL.md` into the
app's custom instructions (or project instructions), and upload the `playbooks/` folder — or
just the one or two playbooks you need — as project files.

**No AI at all.** Open `playbooks/en/` or `playbooks/zh/` and read the card for your situation.
Each one ends with a one-page checklist you can take into the meeting.

## Try asking

- "Our largest customer wants 30% off at renewal or they'll leave. What do I do?"
- "My co-founder wants a 50/50 split. Is that a problem?"
- "I've interviewed 15 people and everyone says they'd use it. Is that enough?"
- "This industry report says the market is $40B and growing 30% a year. How much should I trust it?"
- "We have four months of cash and the next round isn't coming. What now?"

## How the content was made

Each playbook is a synthesis of several established schools of practice, written fresh in
plain language. Every statement was checked against its sources for overreach, missing
caveats and wrong attribution; examples were anonymised; and contested points are shown from
both sides rather than flattened into one answer.

## Roadmap

Situations founders ask about that the twelve playbooks don't yet cover well: fundraising
mechanics (bridges, term sheets, a lead investor pulling out), runway and cash planning, and
dependence on a single large customer. Real cases help decide what comes next — see
*Contributing*.

## Disclaimer

General guidance for thinking through decisions — not legal, tax, accounting or investment
advice. The equity playbook follows mainland China company and tax law as generally practised
and may be out of date; check current rules with a qualified local adviser before acting.

## Contributing

The most useful contribution is a real situation the playbooks handled badly: open an issue
describing what you asked, what you got, and what was missing or wrong.

## License

[MIT](LICENSE)
