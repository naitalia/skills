---
id: 2
slug: mvp-and-scope
title: MVP and Product Trade-offs
when:
  - The product has been in the works for months and I keep feeling a few more features are needed before it's presentable
  - Customers and colleagues ask for "just one more feature" every day, and I can't tell what to build first or what to refuse
  - A competitor just shipped a feature and the team says we need it too
  - The product is live, some people pay and some praise it, but I can't tell whether it has really found its market
  - Users want us to build a whole, complete thing and we have very few people
  - I'm building a platform, neither side has any users yet, and I can't get it started
---

# MVP and Product Trade-offs

The line for shipping a first version isn't "the features are all there" but "we can start learning from customers": almost nothing about customers is learned during development and testing, so the first version should shrink to just what delivers your core promise. The same logic applies after launch: don't add features by default; if you add, queue them and treat them as experiments. To judge whether you've found the market, look first at how many people you keep and how upset users would be to lose the product, not at revenue. For how to validate demand before launch, see "Direction and Demand Validation".

## Quick take

- **Key questions**: What is the core promise we make to customers, and is this feature delivering it or did I add it in passing while polishing the demo? Do I want to build it because I understand users, or only because competitors have it and someone said it's good? Is my product one-time value or something people use again and again, and is anyone paying without using it?
- **Preferred plays**:
  - **Shrink the first version to the point where learning can start**: label each feature must have, nice to have or not needed, and include one only if it's truly needed; shrinking isn't shoddiness, you still have to deliver the core promise.
  - **After launch, don't add by default; queue and validate**: triage requests, ask customers why they want something rather than building the fix they proposed, treat what's worth building as experiments, and cap work in progress.
  - **Judge whether you've fit the market**: first sort out one-time value versus repeat use and watch activation or retention, then ask users how disappointed they would be to lose it; don't look at revenue alone, it is only a first-level validation.
- **Common traps**: Believing the first version must be complete before it goes out, or polishing the demo until it keeps growing; shrinking into shoddiness; looking only at revenue, or scaling before early pull exists.
- **Evidence**: All of it is practitioners' personal experience and single cases, with no controls and no independent replication; the figures on the card are mostly spoken estimates, secondhand references or the proponents' own conversions.
- **Not in this card**: How much to cut is enough, and how long until launch (the sources give a test, not a number of days or features); when to cut losses or pivot.

## Ask these first

1. What is the core promise we make to customers? Is this feature delivering it, or did I add it in passing while polishing the demo?
2. Behind the big solution the user asked for, which specific moment is the real need? If we served only that moment, what would the narrow version look like?
3. Am I only working out how to make some component better, without ever asking why it needs to exist?
4. Do I want to build it because I understand users, or only because competitors have it and someone said it's good?
5. Have the existing features been properly tested and their problems fixed? Have I counted the cost of adding this one?
6. Is my product one-time value, or something people must use again and again? Is anyone paying without using it?

## Plays

### 1. Shrink the first version to the point where learning can start

Development and QA teach you almost nothing about customers; most customer learning happens after release, so the later you ship, the later learning begins. Those two stages can't be removed, but the time from collecting requirements to release can be shortened. Shrinking isn't the same as being shoddy — you still have to deliver the core promise.
There is a separate reason too: a complex system has to grow out of a simple one that works, because the parts need time, while running, to test one another. Same practice, different reason.
1. Start from zero and go through every feature; include one in the first version only if it's truly needed, beginning with the features that solve the customer's number-one problem.
2. Label each feature in the demo as one of three kinds: must have, nice to have, or not needed. Throw out the "not needed", put the "nice to have" on a backlog, and treat features that other must-haves depend on as a separate case; then repeat for the second and third biggest problems.
3. For customer requests (say, integrating with other software they use), study them and decide by importance whether to add them.
4. At launch, tell customers up front that it costs money but bill at month's end; outside a free trial don't ask for a credit card on the spot, and don't hurry to prepare multiple plans. Don't optimize servers, code or databases — the goal is learning, not optimization.
- Done when: every feature has a label, the backlog holds the "nice to have" items, and the pre-launch to-do list has no performance optimization (judgment).
- The moment you're most tempted to pad the first version is right after solution interviews, when customers seemed to like it. The labels also come from customers' reactions in interviews; with a small sample and polite customers, it's easy to label what they said they want as a must-have (both points are judgment).

### 2. Reduce the big solution to the need at "that moment"

What users propose is sometimes a big solution (this practice is a summary of the source's three examples, not the proponent's own words). Reduce it to the need at one particular moment and build only that; the part you cut becomes a narrow solution or an unobtrusive entry point instead of being deleted outright.
1. Ask: behind this big solution, which specific moment is the real need?
2. Ask: what narrow solution would serve only that moment, and is a complete solution that solves everything really necessary?
3. Could the part you cut become a hidden entry point?
4. Also ask "why does this have to exist at all?" rather than only how to make it better. That question is about whether it should exist; the ones above are about which moment it serves.
- Be clear about why you're cutting: in the source's three examples, some cuts were for security and some to protect the experience of "reaching the other person instantly" — not all were about scope.

### 3. After launch: don't add by default; queue and validate what you do add

The usual reaction is to make the product bigger and fuller, which often backfires: extra features dilute your core promise; the first version only validated the framework, so existing features haven't been proven; every feature has a cost; and you still don't know what customers really want, so treat new features as experiments.
As for stance, say no to new ideas by default and make the proposer make the case (judgment); user feedback only helps you understand what users are thinking — don't treat it as a feature list.
1. When a request comes in, compare it with what matters most right now: is it the right request at the right time? (For example, while the sign-up flow has a serious problem, requests about other steps wait.)
2. Sort it: a small feature, a bug fix, or a feature big enough to be worth telling customers about. Small things that must be done now get done now; the rest queue by priority.
3. For queued items, first ask "is this worth solving?" and kill it if you can't find a good reason. For customer requests, call or meet them and ask why they want it to find the root problem, rather than building the fix they proposed.
4. Cap the number of features in progress at once, starting at the number of co-founders or team members.
5. For the ones worth building, show customers a product mock-up first and start coding only when they're very satisfied; deploy to a few customers first for usability testing; after full release, compare conversion in the week before and after.
- Done when: every request has a destination, work in progress stays within the cap, and most of your time after launch goes to evaluating and improving existing features.
- A very early team of one or two can start by taking only two pieces — triaging requests and the cap on work in progress (judgment; the source doesn't say this).

### 4. Judge whether you've fit the market: first how many you keep, then whether they'd be upset to lose it

Revenue is only a first-level validation: many customers pay without using the product — sometimes the company pays for them, sometimes they forgot to cancel an automatic charge.
1. First sort out the type: for one-time-value products (wedding photography, novels) watch the activation rate; for products people come back to (software services, social networks, restaurants) watch retention.
2. Review conversion at a fixed time each week and find the step with the biggest drop-off; rank the features still to build; make bold hypotheses but test them only with the simplest version; redo or remove features that don't work.
3. Watch the number of retained users. The proponent's bar is keeping about forty percent of activated users, month after month.
4. Once you reach that line, ask users one question: how would you feel if you could no longer use this product? The options are very disappointed, somewhat disappointed, no difference, and I no longer use it. If more than forty percent say "very disappointed", it is quite possibly a must-have. The question only tells you whether early pull exists, not how to get it; you need enough respondents, and with business customers don't ask it this directly, as it can irritate them.
5. Without early pull, don't rush to scale; once you have it, shift focus at once to making the company sustainable.
6. A different kind of signal is word of mouth: listen to how users describe you in public. The proponent holds that "fun" and "thrilling" spread on their own, while "saves money" and "a handy tool" may not; if nobody spontaneously calls a new product fun on a public platform, treat it as unable to spread. This tests whether people will speak up for you; the steps above test whether they could do without you.

### 5. Platforms and network-effect products: prove value inside a small circle first

The same process works for these two kinds of product, but the start has to be adjusted: prove value on a small scale first and don't rush to spread out.
1. Network-effect products: the first milestone is building something people want, measured by repeat use and engagement; validate on a small scale, then use word-of-mouth to push toward the tipping point, and find a way to survive until you get there.
2. Marketplaces: draw up a separate business-hypothesis sheet for buyers and for sellers and interview each side; first find an existing small circle where both sides are eager to trade and trading is a hassle, and prototype there rather than starting a new big market.
3. Don't match buyers and sellers automatically; do the matching by hand first and learn which steps suit automation.

## Common traps

- Believing the first version must be complete and solid before it goes out; or, in solution interviews, polishing the demo until it grows and pointless features slip into the first version.
- Shrinking into shoddiness: the activation flow doesn't deliver what the landing page promised, and you only get one first impression.
- Too many features in progress at once; building only the fix the customer gave you; defining "done" as code written (judgment).
- Looking only at revenue, or picking the wrong way to raise it (a one-time buyout license, custom development work); scaling before early pull exists.
- Turning "say no by default" into dogma: its proponent admits that priority calls are often gut feel, so it is not a repeatable process.

## Two schools of thought

**Where demand for new features comes from.** One school: it comes not from research, analysis, discussion or competitors but from understanding users and from your own needs; research helps with refining details, but is meaningless for deciding new features. The other: a founder can't be an objective customer, "I'd use it myself" is no substitute for interviews, and you need falsifiable hypotheses and session-by-session interviews. The two agree on one point: don't ask users which features they want.
How to choose (judgment, based on each side's premises): the first school assumes the builder is a typical user, has watched users for a long time, and is making a new category users can't articulate; if the founder isn't the target user or lacks that accumulated observation, use interviews. The second school's proponent also warns from personal experience: when the target user increasingly resembles you and you lose interest in customers' problems, that's a danger sign.

**Friction at sign-up and payment.** One school: at launch, reduce sign-up friction, delay charging, bill at month's end. The other: when validating willingness to pay, don't make sign-up too easy and ask for written or prepaid commitment. The second school's proponent offers his own compromise: reduce friction, but not at the expense of learning.
How to choose (judgment): the first is about friction at launch, the second about validating payment commitment before you build the first version. The same proponent also recommends charging from day one; read together that probably means stating the price on day one and deferring the billing — that is an inference.

**After launch: improve what exists, or explore something new.** One school: spend most of your time improving existing features. The other: pushing a single goal to the extreme eats up your exploration budget. How to choose (judgment): they don't truly conflict — existing features have only validated a framework, so improving them is itself exploration, while new features should still be run as experiments; don't mix the two quotations.

**Self-reported attitude, or actual behavior.** The "how disappointed" question is self-reported and customers can say untrue things; the proponent's bridge is to read behavioral data such as retention alongside it.

## When this doesn't work

- "Say no by default" and "serve only the main scene" come from a team with a huge user base that was already ahead; what a challenger should do about a feature that "everyone else has and customers are clearly leaving over" isn't addressed. Hiding an entry point for a small minority may, with few users, mean hiding it from all of your early users (judgment).
- The "fun" test comes from mass-market social products; word of mouth for business tools often happens in private channels, and silence on public platforms doesn't mean nobody uses them (judgment).
- The examples and tools are all software. Where a release is hard to take back (regulated, hardware, one-off delivery), shipping early costs something different (judgment).
- When a proven approach can be reused as is, there's no need to grow slowly from a simple version; and the source gives no test for what counts as "simple" or "working" (judgment).
- The forty percent line may not mean the same for one-time-value products; with a small sample it is more a direction than a verdict; with only a few dozen users a week, weekly conversion may swing more than it signals (judgment).

## Examples

- Three trade-offs in a mass-market messaging product: users wanted their data in the cloud, so it only built data transfer for when you change phones; users complained typing on a phone was tiring, so it skipped a full computer version (which would make people stop trusting that the other person would get the message instantly) and made an add-on that only borrows the computer keyboard for typing, adding a web version with an interface only later; in the feed you could post only photos, with the entry for posting words alone tucked away somewhere unobtrusive. The source describes the choices and reasons, not the results.
- A founder's consumer product had a fair number of mothers sign up, pay and praise it, yet it wouldn't catch on with a wider group: the target users were too busy to pay attention to it, and in the early interviews they had kept cancelling and rescheduling, which wasn't taken seriously at the time. The founder eventually found the company becoming more technology-driven, the target user more and more like themselves, and their interest in customers' problems gone, and sold the company to its first customer. All of this is the founder's own after-the-fact account; the main reason for leaving was the founder's own state, so don't read it simply as "the product didn't fit the market".

## How solid is the evidence

- These sources are all practitioners' personal experience and single cases, with no controls and no independent replication; one is a successful product leader's after-the-fact spoken account in which some figures were reconstructed from context.
- The forty percent line comes with only a conclusion and one passing note; who did the comparison and what the sample was made of aren't stated, and "keep forty percent of activated users month after month" is the proponent's own conversion.
- "The vast majority of new ideas should be rejected" and "most of our old features could be cut" are spoken estimates; the in-progress cap equal to the number of co-founders cites only a single outside reference on development process.
- The "fun" test is the proponent's own experience-based judgment with no way of measuring it, and his comparison of paying versus saving money is stated hypothetically, not as an experiment. The proponent says the product wasn't about making friends, yet in his own story about getting friends to install it, what drew them was perhaps curiosity about meeting people — his account of motive is after-the-fact (judgment).
- The platform examples, and the examples for asking why something has to exist, are all successes, with no failures that did the same thing for comparison.
- An opposing view says to think the logic through before acting and not to learn by trying; but its main supporting argument was found to contain a factual error about history and has been set aside, so it is no rebuttal of "build something small first" (judgment).

## One-page checklist

- [ ] I can state our core promise to customers in one sentence, and every feature in the first version delivers it
- [ ] Every feature in the demo is labeled must have, nice to have or not needed, and the backlog holds the rest
- [ ] For each big request I've written down "which one moment it serves"
- [ ] Requests are triaged, killed ones have reasons, customer requests were traced to the root problem, and there's a cap on work in progress
- [ ] I know whether mine is one-time value or repeat use, watch the right metric, and have checked whether anyone pays without using it
- [ ] I'm not scaling before early pull exists

## Not covered by this card

- How much to cut is enough: the sources give a test, not a number of days or features, so "how long until launch" has no answer here
- When to cut losses or pivot: how long retention below forty percent counts as a mismatch, and after how many iterations to switch
- How to build a first version of hardware, services or large enterprise deals
- Fit-metric thresholds for low-frequency or one-time-value products; how to read the question and retention when early users are very few
- What to do when a big paying customer insists on a feature (no feature, no deal); whether to follow when a competitor ships one
- Who decides when the team disagrees about features
- Timing of charging and pricing, see "Pricing"; the pace of expansion and when to hire after fit
