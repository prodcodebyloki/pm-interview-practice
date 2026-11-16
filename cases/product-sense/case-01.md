<!-- PROVIDED BY USER. Template fields at the top are drawn only from the user's case text. The user's full worked answer is preserved below "Model answer". -->
<!-- INTERVIEWER ONLY. Never read anything below "Opening question" aloud, except reveal-if-asked facts when asked. -->
# case-01: Rippling AI Usage Tracking, Provisioning and ROI

- **Company / product:** Rippling (HR, payroll, IT, devices and spend management on one employee data model)
- **Intended difficulty:** hard (new, cross-functional problem; heavy on metrics and ROI)
- **Skills tested:** D2, D3, D4, D6, D7

## Context given to the candidate
None beyond the question. The candidate should set their own assumptions.

## Opening question
> "You're a PM at Rippling. Design a product that helps companies track, provision and measure the ROI of the AI tools their employees use."

## Reveal if asked
- **What Rippling has:** HR, payroll, IT, devices and spend on one employee data model. It holds identity and SSO (who has which app), card and expense data (what it costs), and people data: team, role, level, manager, tenure, start date, and compensation.
- **Platform:** building inside Rippling is fine. It does not need to be a standalone product.
- **Market and size:** U.S. is fine. Company size is the candidate's choice; mid-size companies (roughly 100-1,000 employees) are a typical customer.
- **Which AI tools:** chat assistants, coding assistants, and AI add-ons inside existing SaaS apps. In-house models are the candidate's call to scope out.
- **How tools get adopted today:** personal and corporate cards, expenses, free tiers, add-ons inside existing apps, Slack seat requests, and vendor consoles. Sometimes shared logins.
- **Competitors:** SaaS management platforms (Zylo, Productiv, Torii, Zluri), spend tools (Ramp, Brex), and each vendor's own admin console.
- **Scale, if asked for numbers (illustrative):** a 400-person company with 300 AI assistant seats at $30 per seat per month, of which about 180 are active weekly.

## Hold back
- **Vendor data is uneven.** Some tools expose rich usage APIs and others expose nothing. Share only if the candidate asks how usage data is obtained.
- **Employee trust.** Tracking can feel like surveillance and suppress adoption. Never raise it unless the candidate does; it is a key signal if they scope to metadata unprompted.
- **Self-reported time saved runs high.** Share only if the candidate proposes self-reports and asks about accuracy.

## Follow-up questions
<!-- Drawn from the case text. The interviewer asks only these, plus bare prompts like "Why?". -->
- **Stage 1 Motivation →** "How is this different from what a vendor's admin console or a spend tool already shows?"
- **Stage 2 Segmentation →** "Why AI program owners rather than finance or security?" · "Why value proofers over spend controllers?"
- **Stage 3 Problems →** "Why ROI blindness over blind spots or seat mismatch?" · "What's the root cause?"
- **Stage 4 Solutions →** "Why is this defensible against a SaaS management tool?" · "How do you know the savings are real?" · "How would a customer actually calculate ROI?"
- **Stage 5 Metrics →** "Which one metric would you watch weekly?" · "How does this make Rippling money?"

## Curveball options
- **Problem or solution stage →** "Won't employees feel surveilled by this?" (Skip it if the candidate already scoped to metadata only.)
- **Solution stage →** "Some AI vendors expose rich usage APIs and others expose nothing. What happens to your v1?"
- **Metrics stage →** "Utilization is up but ROI is flat. Why?" or "Employees are using AI less since launch. What now?"
- **Metrics stage (alt) →** "Rippling's AI tab has strong discovery but weak weekly usage by finance. What do you do?"

## Model answer notes
- Strong segment: AI program owners, specifically the "value proofers" (IT or ops-led, must show the AI investment is working). Persona: Marcus.
- Key problem: ROI blindness. The root cause is a missing join across vendor usage, billing, identity and HR, not missing analytics.
- Strong v1: an AI Scorecard on a unified inventory, plus a thin slice of idle-seat reclamation as the hard-dollar win. Privacy by design: metadata only, team-level reporting.
- Strong metric: a north star of verified-value AI spend %, with guardrails on employee trust, data quality and wrong reclamation.
- The practice variations at the end are for your own study. They are never asked in a session.

---

## Model answer (teardown mode only)

### Product Sense Case Study: Rippling AI Usage Tracking, Provisioning and ROI

A worked answer using the five-step product sense framework, centered on tracking and provisioning AI tools across a company and measuring their ROI. Product details are based on general public knowledge of Rippling; all numbers are illustrative placeholders you should adapt, not real company data.

#### The question

"You're a PM at Rippling. Design a product that helps companies track, provision and measure the ROI of the AI tools their employees use."

This is a strong case because the problem is new, painful and cross-functional: IT, finance and HR each own a piece of it, and no one sees the whole. Rippling's differentiator is exactly the join between those pieces, since employee records, app access, devices and spend already sit in one data model. A good answer stays on one user and one problem, and shows how the unified data makes the ROI claim credible.

#### Time plan (35 minutes)

| Step | Section | Time |
|---|---|---|
| 0 | Assumptions + game plan | 3 min |
| 1 | Product motivation | 4 min |
| 2 | Segmentation | 8 min |
| 3 | Problem identification | 8 min |
| 4 | Solution + v1 + risks | 9 min |
| 5 | Success metrics | 3 min |

#### Step 0: Assumptions and game plan

"I'll assume I'm a PM at Rippling, which brings HR, payroll, IT, devices and spend management together on one employee data model, and I'll build a new capability inside that platform rather than a standalone product.

Three assumptions. One: I'll start with the U.S. and companies of roughly 100 to 1,000 employees, where AI adoption is fast but dedicated AI governance teams don't exist yet. Two: I'll focus on AI tools employees use for work, meaning chat assistants, coding assistants and AI features inside SaaS apps, not AI models a company builds itself. Three: I'll track usage metadata such as who, which tool, how often and how much it costs, not prompt or output content.

My plan: why this matters and the mission, then the ecosystem and one target segment, then the user's journey and one problem to prioritize, then solutions, a v1 and risks, and finally how I'd measure success. Does that work for you?"

**Why this works:** the third assumption is a deliberate scoping and trust decision. It pre-empts the surveillance objection the interviewer is likely to raise and signals product judgment early.

#### Step 1: Product motivation

**The need.** Employees now adopt AI tools faster than any company can buy, approve or measure them. Teams expense chat subscriptions, engineers install coding assistants, and existing SaaS apps ship AI add-ons with their own price tags. Leaders end up asking three questions they cannot answer: Who has access to what? What are we paying? What are we getting back? The deeper need is confident, accountable AI adoption: spending where AI helps, stopping where it doesn't, and doing it without creating a security or trust problem.

**Strategic and competitive context.**
- Rippling's bet is that HR, IT and finance data belong in one graph. A hire triggers payroll, a laptop, app access and a card; a role change should change entitlements. AI tools are the newest and fastest-growing category of apps and spend inside that graph.
- Rippling already holds the three ingredients AI ROI needs: identity and access (who has which app), spend (what it costs), and people data (role, team, manager, tenure, and the compensation data to turn time saved into dollars).
- Competitors: SaaS management platforms such as Zylo, Productiv, Torii and Zluri (strong on app and license discovery, weaker on HR context), spend tools such as Ramp and Brex (see the money, not the usage), and each vendor's own admin console (accurate for one tool, blind to the rest).
- The wedge: a vendor console can tell you Dana used the tool 40 times. Only a platform that also knows Dana's team, role, cost and tenure can tell you whether that usage was worth the seat.

**Mission statement (placeholder):**
"To help every company adopt AI deliberately: the right people have the right tools, no money is wasted, and leaders can prove the value."

**Check-in:** "Does this framing work before I get into who we're serving?"

#### Step 2: Segmentation

**Ecosystem players**
- AI program owners: IT, business systems or ops leaders accountable for rolling out and governing AI tools
- Finance leaders (CFO, FP&A): own budget and want evidence behind renewals
- Security and compliance: worry about shadow AI, data exposure and vendor risk
- Managers and employees: use the tools, request seats, and are the ones being measured
- AI vendors: supply tools, usage APIs and admin consoles; shape what data is available

"I'll focus on AI program owners. They are the daily operators and the buyers of this product, they sit between finance, security and employees, and if they get a trustworthy view, every other group benefits. Does that make sense before I segment?"

**Segmentation heuristics**
What drives a program owner's behavior is the question they are being held to. I'll segment on that primary motivation, then check size of company, how many AI tools are in use, and whether they report to finance, security or the executive team.

**Three mutually exclusive segments**

| Segment | Primary job-to-be-done | Reach | Underserved degree |
|---|---|---|---|
| Spend controllers | Finance-led; stop paying for duplicate or unused AI seats | High | Medium: spend and SaaS management tools already cover much of this |
| Risk guardians | Security-led; find shadow AI and control who can use what | Medium | Medium-High: security tools see access, not business value |
| Value proofers | IT or ops-led; own the rollout and must show leadership the AI investment is working | High | Highest: nobody connects usage and cost to outcomes |

**Mutual exclusivity check:** the segments differ by the question their owner must answer ("what can we cut?", "what is exposed?", "is it working?"), and each needs a different primary screen and success metric. A person may care about all three, but only one is the question their boss is asking them this quarter.

"I'll prioritize value proofers. High reach, most underserved, and they are the group most likely to want provisioning and measurement in one place, which is exactly what Rippling's unified data enables. Solving their problem also delivers most of what spend controllers and risk guardians need."

**Persona**
Marcus, 41, Head of IT and Business Systems at a 400-person software company. In the past year, teams adopted four chat assistants, two coding tools and a dozen AI add-ons inside existing apps. The CEO just asked at a leadership meeting, "We're spending real money on AI. What are we getting for it?" Marcus has a spreadsheet stitched from card statements, vendor admin exports and a Slack channel of seat requests, and he doesn't trust it.

#### Step 3: Problem identification

**Marcus's journey: the lifecycle of an AI tool in his company**
1. Discover: learns that a team has been using a new AI tool, often months after it started, via a card statement or an offhand comment.
2. Evaluate and approve: checks security basics and budget; no standard way to compare it with the three similar tools already in use.
3. Provision: assigns seats through a Slack request, a vendor console and sometimes a shared login; new hires wait days, and role changes rarely update access.
4. Monitor: exports usage from each vendor in a different format and tries to match emails to people and teams.
5. Renew or reclaim: at renewal, decides by gut feel; idle seats keep billing because nobody has time to chase them.
6. Report: builds a one-off slide for the CEO and CFO, with usage counts but no outcomes.

**Three problems**
1. **Blind spots.** Marcus struggles to know which AI tools are in use and by whom, because adoption happens through personal cards, free tiers and add-ons inside existing apps, so unmanaged tools carry data and cost risk he only finds out about late.
   - Frequency: High (continuous). Severity: High (security exposure, duplicate spend).
2. **Seat mismatch.** Marcus struggles to match seats to the people who will use them, because access is granted by request and rarely revisited, so new hires wait, leavers keep access, and idle seats keep billing.
   - Frequency: High (every hire, change and renewal). Severity: Medium-High (direct waste plus slow ramp).
3. **ROI blindness.** Marcus struggles to show whether AI spend is paying off, because usage sits in vendor consoles, cost sits in finance systems and people data sits in HR, so he can report activity but not value, and renewals and budgets are decided without evidence.
   - Frequency: Medium (quarterly reviews, renewals, budget cycles). Severity: Very high (budget cuts or unchecked spend, and lost credibility with leadership).

"On severity and frequency I'll prioritize ROI blindness. It is the most underserved, the moment of highest stakes for Marcus, and the one my platform is uniquely placed to solve. It also depends on the other two: you can't prove ROI without knowing who uses what, and the savings from fixing seat mismatch are the first hard-dollar proof of value. So the solution must include the data foundation."

**Root cause (systems thinking):** the facts needed for ROI live in four systems that never meet: vendor usage, billing, identity and HR. Marcus is doing the join by hand. The problem isn't missing analytics; it's a missing join.

#### Step 4: Solution development

**Three distinct solutions**
1. **AI Scorecard on a unified inventory.** Rippling auto-discovers AI tools from SSO, card and expense data, then joins vendor usage, spend and people data into a per-tool and per-team scorecard: seats paid, seats active, cost per active user, adoption by role, and an estimated net value.
2. **Policy-based provisioning and reclamation.** Rules tied to HR events assign AI seats by role and team at hire or transfer, request-and-approve in one place, and automatically flag or reclaim seats idle for a set period and revoke access at exit.
3. **Structured AI pilots.** Companies run a rollout as an experiment: pick a team, set a baseline metric, give half the team access, and Rippling compares outcomes between cohorts before a wider purchase.

**Impact vs. effort**

| Solution | Impact | Effort | Rationale |
|---|---|---|---|
| AI Scorecard + inventory | High | Medium | Directly answers "what are we getting?"; the join across identity, spend and HR is Rippling's strength |
| Provisioning + reclamation | High | Medium | Creates hard-dollar savings and makes the scorecard actionable; builds on existing app and device provisioning |
| Structured AI pilots | High | High | Most rigorous ROI evidence, but needs experiment tooling and customer discipline; better as a later phase |

"I'll prioritize the AI Scorecard on a unified inventory, with a thin slice of reclamation in v1 so insights turn into savings, not just charts. Pilots become the v2 roadmap. It's defensible because a point solution sees only usage, only spend or only access, while Rippling can tie one person's seat, cost, role and tenure together, and enforce the result by changing their access."

**V1 definition**
- **Who:** U.S. companies of 100 to 1,000 employees already on Rippling IT or Spend, starting with a design-partner cohort of 20 to 30 customers.
- **Data sources:** Rippling identity and SSO events, card and expense transactions, HR attributes (team, role, level, manager, start date), and admin APIs from the 8 to 10 most common AI tools (chat assistants, coding assistants and AI add-ons in major SaaS apps).
- **Inventory:** auto-discovered list of AI tools with status approved, under review or unapproved, owner, seat count and monthly cost.
- **Scorecard per tool and team:** paid vs. weekly-active seats, utilization %, cost per active user, trend, and adoption by role.
- **Value estimate:** the admin picks a value method per tool: manager-reported hours saved, a baseline team metric (for example support tickets closed or pull-request cycle time), or both. Rippling converts time to dollars using aggregated, team-level loaded cost, never individual pay.
- **Action layer:** one-click "reclaim idle seats" (no activity in 30 days) with manager notice, plus a single seat-request flow that auto-approves by policy.
- **Privacy by design:** metadata only, no prompt or output content, no individual performance ranking, and reports at team level with a minimum group size (for example 5) so no one is singled out.
- **Out of scope for v1:** automatic cancellation, international, in-house models, and automated pilots.
- **Discovery:** shows up as an AI tab in Rippling IT and Spend, with a first-week email digest to admins summarizing tools found and idle-seat savings available.
- **Vision:** continuous provisioning by role and tenure, structured pilots with control cohorts, renewal recommendations, and benchmark comparisons across similar companies.

**Risks and mitigations**
- **Risk: employees feel surveilled.** Tracking AI use can erode trust and suppress adoption. Mitigation: metadata only, team-level reporting, transparent employee-facing notice of what is collected, and no use in performance reviews by default.
- **Risk: ROI numbers aren't credible.** Self-reported time saved is biased. Mitigation: show confidence labels, apply a realization haircut, favor baseline metrics where available, and let finance adjust assumptions.
- **Risk: incomplete or uneven vendor data.** Some tools expose rich usage APIs and others expose nothing. Mitigation: show coverage honestly (for example "72% of detected spend has usage data"), and use SSO and browser-level signals as fallback.
- **Risk: wrong reclamation.** Pulling a seat from someone who uses the tool in bursts. Mitigation: manager notification, grace period, and one-click restore.

**Close (tie back to the mission)**
"To summarize: companies are adopting AI faster than they can govern it. I focused on value proofers like Marcus, whose core problem is that usage, cost and people data never meet, so he can't prove ROI. I proposed an AI Scorecard on a unified inventory, with idle-seat reclamation as the first hard-dollar win, powered by Rippling's identity, spend and HR data. That serves the mission of deliberate AI adoption where leaders can prove the value. Now I'll cover how a customer measures ROI and how I'd measure our own success."

#### How a customer measures AI ROI

The scorecard needs a defensible ROI model. Say it out loud in the interview: benefits minus costs, divided by costs, with every input traceable to a data source.

**ROI = (Benefits − Costs) / Costs**

| | Included | Data source |
|---|---|---|
| Benefits | Time saved on active users (hours × loaded hourly cost × realization factor) | Usage from vendors and SSO; manager surveys; team-level cost from HR |
| Benefits | Hard savings from reclaimed or consolidated seats | Seat counts and invoices |
| Benefits | Outcome gains on a baseline metric (cycle time, tickets closed, quality) | Integrations and admin-defined metrics |
| Costs | Licenses and usage-based fees | Card, expense and invoice data |
| Costs | Enablement, training and admin time | Admin estimate |
| Costs | Security and compliance overhead | Admin estimate |

**Worked example (illustrative numbers)**
A 400-person company holds 300 AI assistant seats at $30 per seat per month. Rippling finds 180 seats active weekly and 120 idle for 30+ days. Active users self-report 2 hours saved per week over 46 working weeks, at a $55 loaded hourly cost, and the company applies a 50% realization factor because self-reports run high. Enablement costs $20,000 per year.

| Line item | Before reclamation | After reclaiming idle seats |
|---|---|---|
| Seats paid | 300 | 180 |
| License cost | $108,000 | $64,800 |
| Enablement cost | $20,000 | $20,000 |
| Total cost | $128,000 | $84,800 |
| Gross time value (180 users × 2 hrs × 46 weeks × $55) | $910,800 | $910,800 |
| Benefit after 50% realization | $455,400 | $455,400 |
| Net value | $327,400 | $370,600 |
| ROI | 256% | 437% |

**The lesson:** the first lever is rarely a new feature. Reclaiming 120 idle seats saves $43,200 a year and lifts ROI by 181 points without changing anyone's productivity. That is the hard-dollar proof that gets a program owner credibility, and why provisioning belongs in the same product as measurement.

**What to caution about:** the benefit side is an estimate. A good product shows the assumption behind every number, labels confidence, and lets finance change the realization factor instead of hiding it.

#### Step 5: Success metrics

Structure: goal → north star → input metrics → business impact → guardrails → how to evaluate. There are two lenses to keep apart: the customer's AI ROI (what the product helps them achieve) and Rippling's success (whether customers adopt and keep the product).

**Goal**
Help customers move AI spend from unmanaged to managed and measurably valuable, which deepens Rippling's role as the system of record for people, access and spend.

**North star metric**
Verified-value AI spend: the percentage of a customer's AI spend that goes to seats actively used (weekly) and tied to a measured outcome in the scorecard.

Why this metric: it captures coverage (we see the spend), provisioning quality (seats are used), and ROI evidence (value is measured), it moves only when customers act, and it is hard to inflate by showing more dashboards.

**Metric tree**

| Layer | Metric | Definition | Illustrative target |
|---|---|---|---|
| North star | Verified-value AI spend % | Spend on active, outcome-linked seats ÷ total detected AI spend | 60%+ within 6 months of onboarding |
| Coverage | Spend coverage | Detected AI spend ÷ audited total (card, expense, invoices) | > 90% |
| Coverage | Usage-data coverage | % of detected spend with usage data from vendor, SSO or other signal | > 70% |
| Coverage | Shadow AI discovery | Unapproved tools found per customer in first 30 days | Directional; then falling as policy takes hold |
| Provisioning | Seat utilization | Weekly-active seats ÷ paid seats | +15 to 25 pts vs. baseline |
| Provisioning | Time to provision | Request to working access | < 1 business day |
| Provisioning | Offboarding revocation time | Exit date to AI access removed | Same day |
| Provisioning | Idle spend reclaimed | $ saved from reclaimed or consolidated seats | 10 to 20% of AI license spend |
| ROI | Cost per active user | License + usage cost ÷ weekly-active users | Falling or stable as adoption grows |
| ROI | Tools with measured value | % of tools with a value method configured | > 70% of spend |
| ROI | Customer-reported ROI | Net value ÷ cost, per tool and in total | Positive on > 80% of managed spend |
| Adoption | Weekly active admins and viewers | Admins, finance and execs opening the scorecard | Growing; finance share rising |
| Adoption | Actioned insights | Reclaims, reassignments, renewals and cancellations made in product | 3+ per customer per quarter |
| Business | Attach and expansion | Share of Rippling IT/Spend customers using AI tab; added modules | Directionally higher vs. non-users |
| Business | Retention and NPS | Logo retention and admin NPS among AI tab users | Higher than comparable non-users |

**Funnel view**
Customers eligible → data sources connected → inventory reviewed → value method configured → first action taken (reclaim, reassign, renew) → scorecard shared with finance or leadership.

Use it to find the leak: low connection means integration friction, low value configuration means the ROI setup is too hard, low sharing means the output isn't convincing.

**Guardrail metrics**
- Employee trust: pulse survey on comfort with AI usage tracking, opt-out or complaint volume, and any drop in AI adoption after launch (a sign that tracking is chilling usage).
- Data quality: discovery false-positive rate, usage-match accuracy (email to person), and connector failure rate.
- Wrong reclamation: seats restored within 14 days of reclaim; target low and falling.
- Estimate integrity: share of ROI figures carrying a confidence label, and finance override rate on assumptions.
- Security and privacy: access or data incidents and compliance escalations (target: zero).
- Time to value: days from onboarding to first scorecard and first action.

**How to evaluate**
1. Design-partner cohort first. Launch with 20 to 30 customers, interview admins and finance partners every two weeks, and check whether the numbers survive a CFO's questions.
2. Staged rollout with a holdout. Randomize at the company level, stratified by size and number of AI tools, and compare verified-value spend, idle spend and retention for at least two billing cycles.
3. Backtest the discovery. Compare detected tools with a manual audit at several customers to measure recall and false positives before widening.
4. Decision rule. Expand if coverage and precision clear their thresholds, actioned insights are growing, and the trust guardrails hold. Otherwise fix data quality before adding features.

**Common metrics follow-ups**
- "Utilization is up but ROI is flat. Why?" Active use may be low-value or already counted. Segment by role and task, check which tools lack a baseline metric, and revisit the realization factor.
- "Employees are using AI less since launch." A trust red flag. Review communications, confirm no content is collected, and consider employee-facing transparency before any further tracking.
- "How do you know the savings are real?" Distinguish hard savings (invoiced seat reductions, verifiable) from soft benefits (time saved, estimated), and report them separately.
- "Which one metric would you watch weekly?" Actioned insights per customer, because it is the leading indicator of whether the scorecard changes decisions; the north star lags by billing cycles.
- "How does this make Rippling money?" It raises retention and attach of IT and Spend, opens a new paid module, and makes Rippling the system customers use to govern AI as well as people.

#### Final takeaways
1. Anchor on one persona and one problem. Everything traces to Marcus's "usage, cost and people data never meet, so I can't prove ROI."
2. Use Rippling's unique asset. The join across identity, spend and HR is the moat; vendor consoles and spend tools each see one slice.
3. Pair measurement with action. Reclaiming idle seats gives hard-dollar proof and makes the scorecard more than a dashboard.
4. Design for trust. Metadata only, team-level reporting and transparency decide whether employees keep using AI.
5. Separate hard savings from estimated value in ROI, and show the assumptions behind every number.
6. Metrics flow from the goal: north star, coverage, provisioning, ROI, adoption, guardrails, then an experiment that fits the rollout.

#### Practice variations
- "Design the offboarding experience for AI tools and data when an employee leaves."
- "How would you decide which AI tools Rippling should natively integrate first?"
- "Build a spend-governance feature for usage-based AI API costs."
- "Rippling's AI tab has strong discovery but weak weekly usage by finance. What do you do?"
