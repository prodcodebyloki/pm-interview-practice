<!-- PROVIDED BY USER. Source: distilled from Ben Erez's guide in Lenny's Newsletter. Content preserved; formatted as Markdown. -->
<!-- INTERVIEWER NOTE: Never quote, hint at, or paraphrase this file during mock mode. Section 9 is a model answer: use it only in teardown mode, or when the user explicitly asks for a hint. -->

# Product Sense Interview: Step-by-Step Framework

An action-oriented playbook expanded from Ben Erez's guide in Lenny's Newsletter. It includes a full worked example on Claude Artifacts.

## 1. The big picture

A product sense (PS) interview tests whether you can identify user needs, articulate problems, and craft solutions, with empathy, creativity and structure. It runs about 45 minutes, leaving roughly 35 minutes for the core exercise.

The interviewer is usually a busy PM with a rubric. Your job is to make their job easy by generating clear, easy-to-spot signals for each rubric dimension. You need a solid pass on every dimension; brilliance in one cannot rescue weakness in another.

### The five dimensions and the flow

| Step | Dimension | What you prove | Time |
|---|---|---|---|
| 0 | Clear communication | You lead with structure and stay adaptable | 3-5 min |
| 1 | Product motivation | You understand why the product exists | 3-5 min |
| 2 | Segmentation | You can define and prioritize an audience | 8-10 min |
| 3 | Problem identification | You find real, prioritized pain points | 8-10 min |
| 4 | Solution development | You brainstorm, choose, and scope a v1 | 8-10 min |

**The golden thread:** mission statement → segment → persona → problem → solution → v1. Every decision should visibly connect back to the one before it.

### The universal rhythm for every section

1. Pause for 1-2 minutes of silent thinking (it's allowed and respected).
2. Walk through your thinking out loud, with signposts ("First... second... so my conclusion is...").
3. Check in with the interviewer before moving on ("Does this make sense before I move to problems?").

## 2. Step 0: Clear communication (the baseline skill)

**Goal:** Start the interview like someone who knows the game. The opening minutes can make or break the interview.

**How to tackle it**
1. Restate the question in one sentence so you and the interviewer are aligned.
2. Set 2-4 assumptions that narrow scope without closing off solutions:
   - Role and context: who you are and which company/product you're working in.
   - Geography: a market to focus on (e.g., U.S. first, global later).
   - Platform and constraints: build inside the existing ecosystem or standalone, mobile vs. web, and so on.
   - Scope boundary: what's out of scope for this exercise (e.g., enterprise customers).
3. Articulate your game plan and ask for a thumbs-up.

**What to say (template)**
> "Before I dive in, here's my plan for our time. I'll start with what the product is and why it matters. Then I'll break down the audience and pick a segment. From there I'll identify key problems and prioritize one. Then I'll brainstorm solutions, pick one, and, if we have time, describe a v1. Does that sound good?"

**What to do**
- Own the structure. Drive the conversation, but stay open to redirection.
- Use explicit waypointing: separate your process ("let me list options") from your conclusion ("I'm choosing option B because...").
- Keep a template with 3-4 placeholder assumptions so you never face a blank page.

**Pitfalls**
- Thinking out loud with no structure; the interviewer has to piece it together.
- Asking "What would you like me to do next?" This signals a lack of ownership.
- Premature narrowing: assuming specific features or user demographics too early.

**How to practice:** Rehearse assumptions and game plan on 20-30 different questions until the opening is automatic. Practice transitions such as "Now that I've set assumptions, here's my plan."

## 3. Step 1: Product motivation

**Goal:** Show you understand the purpose behind a product, not just its features. Spend 3-5 minutes here; don't rush it, and don't over-invest.

**How to tackle it (three parts)**
1. **Product description and value.** What is the product or experience? Which deeper human need does it serve? Why is the world better with it?
2. **Strategic and competitive context.** How does it advance the company's strategy? What market trends matter? Who are the 2-3 key competitors and what makes this offering unique?
3. **Mission statement.** Close with one crisp sentence that will guide every later choice.

**Mission statement rules**
- Specific enough to guide decisions, broad enough to leave room for creative solutions.
- Weak: "Help users be more productive." (too vague)
- Stronger: "Empower anyone to capture and preserve meaningful moments through intuitive photography tools."
- Formula: *Empower [who] to [outcome] through [how/what], so that [bigger impact].*

**What to do**
- Go from feature to need: not "it helps share photos" but "it helps people stay close to loved ones across distance."
- Tie the product to the company mission and to the competitive landscape.
- Tell the interviewer the mission is a "placeholder" you'll use as a North Star.

**Pitfalls**
- Describing features without purpose.
- Mission statements that are too vague or too narrow.
- Strategic misalignment: ignoring the company's strengths, or serving only the company and not users.

**How to practice:** For every app you use, write a one-line human-need description and a mission statement. Study real company missions. Time yourself to stay under 5 minutes.

## 4. Step 2: Segmentation

**Goal:** Think broadly about the ecosystem, then narrow to a specific, vivid target user. Segmentation has three parts.

**Part A: Ecosystem analysis**
1. List 4-5 major stakeholders (users, supply side, partners, internal teams, competitors).
2. Choose one to focus on, with a rationale tied to your mission.
3. Check in: "I'd like to focus on [X] because [reason]. Does that make sense before I define segments?"

**Part B: Segment creation and prioritization**
1. Start with motivations: why do people use (or would use) this product?
2. Pick segmentation dimensions (use 3-5, but say them quickly): primary motivation, behavior patterns and frequency, context of use, expertise level, resource constraints (time, money, space), goals and outcomes.
3. Define exactly three segments. Three thoughtful segments beat many shallow ones.
4. Test mutual exclusivity: could one person belong to two of your segments at once? If yes, refine.
5. Prioritize on a 2x2: reach (how many people) vs. underserved degree (how poorly current solutions serve them). Be decisive: place segments High/Low rather than hiding in the middle. Prefer high reach plus highly underserved.
6. Add a strategic reason: fit with the company's mission and strengths, early-adopter potential, and learning value.

**Part C: Persona**
Bring the chosen segment to life: name, age, role, context, constraints, and a goal. Example shape: "Casey, 29, marketing professional in a city apartment with a small balcony. Excited to start gardening but unsure where to begin."

**What to do**
- Base segments on behavior and motivation, not just demographics ("millennials in cities" is weak).
- Keep the persona specific enough that problems feel authentic.

**Pitfalls**
- Shallow, demographic-only segmentation.
- Skipping ecosystem analysis and jumping straight to end users.
- Overlapping segments, which muddies prioritization.
- Listing too many segmentation properties out loud; keep it brisk so you don't eat the clock.

**How to practice:** Draw ecosystem maps for 5-10 products. Test mutual exclusivity on every practice set. Force yourself to place segments in a High/Low 2x2.

## 5. Step 3: Problem identification

**Goal:** Turn your persona into concrete, emotionally specific pain points and pick the most important one.

**How to tackle it (three parts)**
1. **Map the journey.** Skip generic "before / during / after." Instead walk through a "day in the life" or a product-specific journey with 5-7 stages (e.g., discovery, setup, first use, regular use, troubleshooting, maintenance).
2. **Discover problems.** For each stage ask: Where is the persona confused, slowed, frustrated or anxious? Aim for three well-articulated problems.
3. **Prioritize.** Score each on severity (pain when it occurs) and frequency (how often). Choose one with high scores on both, and explicitly tie it to your mission.

**Needs vs. problems**
- Need (desire): "I want beautiful flowers in my apartment."
- Problem (obstacle): "It's hard to find flowers that thrive in my apartment's limited light."
- Write problems in the form: *"[Persona] struggles to [task] because [cause], which leads to [consequence/emotion]."*

**What to do**
- Be specific about context, emotion and consequence.
- Look for root causes, not just symptoms.
- Say the scoring out loud ("high frequency, high severity") with a one-line justification each.

**Pitfalls**
- Confusing needs with problems.
- Generic journeys that fit any product.
- Problem-solution conflation ("users need a better algorithm" is a solution, not a problem).

**How to practice:** Sketch an hour-by-hour day for different personas. Convert 5 features you use into "I struggle with Y because Z" statements. For practice questions, find at least one problem per journey stage.

## 6. Step 4: Solution development

**Goal:** Show creative breadth, disciplined prioritization, and a concrete, feasible v1.

**How to tackle it (three parts)**
1. **Brainstorm 3 distinct solutions.** They must attack the problem from different angles (e.g., automation, guidance, community), not be variations on one idea. Draw on company strengths, analogies from other domains, and emerging technology used thoughtfully.
2. **Prioritize with impact vs. effort.** Place each in a quadrant, then choose the high-impact, moderate-effort option with clear reasoning. Mention defensibility: why would competitors find it hard to copy?
3. **Define v1 + go-to-market + risks.**
   - v1: the smallest version that proves value (who gets it, what it does, what's explicitly out).
   - Discovery and distribution: how users find it inside existing surfaces.
   - Success metrics: one primary metric plus one or two guardrails.
   - Risks and mitigations: typically two or three.
   - Vision: one sentence on how it evolves beyond v1.

**What to do**
- Connect each solution explicitly to the prioritized problem.
- Close by tying back to the mission statement for a complete narrative arc.
- Use the remaining minute for "what I'd do next" (experiments, expansion).

**Pitfalls**
- Solution jumping (one idea, no alternatives).
- Feature obsession: listing features without linking to the pain.
- Platform mismatch: ignoring the company's unique assets.

**How to practice:** Generate three different solutions to the same problem in five minutes. Map each to a company asset. Rehearse the impact/effort explanation out loud.

## 7. Handling the interviewer

- "Any other problems you'd consider?" is a cue to show more breadth.
- "Why did you prioritize that?" is a chance to explain reasoning with your criteria.
- Redirection is a gift. Adapt quickly, say what you're changing, and continue the structure.
- Short on time? Compress motivation and segmentation, protect problem and solution.
- Pauses are fine. Say "Let me take a minute to think through this."

## 8. One-page cheat sheet

1. **Communicate:** restate, 2-4 assumptions, game plan, check in.
2. **Motivate:** product value, strategy + competitors, mission statement.
3. **Segment:** ecosystem → choose one → 3 motivation-based segments → 2x2 (reach vs. underserved) → persona.
4. **Problems:** day-in-the-life journey → 3 problems → score severity and frequency → pick one, tie to mission.
5. **Solutions:** 3 distinct ideas → impact vs. effort → pick one → v1, GTM, metrics, risks → tie back to mission.

## 9. Worked example: "Tell me about a product you love and how you would improve it" (Claude Artifacts)

Below is how a strong candidate might answer, written in a speakable voice. Details about the product are illustrative and based on general knowledge of how Artifacts work; in a real interview, use what you personally know.

### Step 0: Assumptions and game plan

"I'll talk about Artifacts in Claude, the feature where Claude creates standalone content, like documents, code, web pages, diagrams and small apps, in a dedicated panel next to the chat. I'll assume I'm the PM for Artifacts at Anthropic, working within the existing Claude apps.

Three assumptions. One: I'll focus on the U.S. market first, with global expansion later. Two: I'll improve Artifacts inside the Claude app rather than build a standalone product, to use existing distribution. Three: I'll focus on individual consumer and prosumer users, not enterprise API customers building their own products.

Here's my plan: product motivation, then the audience and a segment, then key problems and one to prioritize, then solutions and a v1. Does that sound good?"

### Step 1: Product motivation

**Product description and value.** Artifacts turn a conversation into something you can use, not just read. Instead of a code block buried in a chat scroll, you get a live app, a formatted document, or a diagram you can iterate on. The deeper human need: people want to move from an idea to a tangible thing, without needing technical skills or a toolchain. Chat is great for thinking; Artifacts are where the thinking becomes a result.

**Strategic and competitive context.** Anthropic's mission is to build safe, helpful AI. Artifacts make Claude more useful for doing, which deepens daily engagement and retention and moves Claude from "answer engine" toward "collaborator that produces work." Competitors include OpenAI's ChatGPT (Canvas), Google's Gemini (Canvas), and app-building tools like Lovable, v0 and Replit. Claude's edge: strong coding and writing quality, instant in-chat iteration, and shareability.

**Mission statement (placeholder):**
"To empower anyone to turn an idea into a working, shareable creation through conversation, so AI becomes a collaborator that produces real work, not just answers."

**Check-in:** "Does this framing work before I move to the audience?"

### Step 2: Segmentation

**Ecosystem players:**
- Creators/builders: individuals making documents, tools, prototypes, visuals with Claude
- Viewers/recipients: people who open artifacts others share
- Developers/engineers: who might export artifact code into real projects
- Anthropic teams: product, safety, infrastructure
- Competing tools and platforms: Canvas, Lovable, v0, Replit, Notion, Figma

"I'll focus on creators, the people making artifacts. They drive all downstream value: if creators succeed, there is something worth sharing and viewers follow. Does that make sense?"

**Primary motivations for creating artifacts:**
- Getting work done faster (documents, analyses, reports)
- Building small tools without coding skills (trackers, calculators)
- Prototyping or learning (testing app ideas, exploring concepts)
- Communicating ideas visually (diagrams, dashboards, explainers)

**Segmentation dimensions:** technical skill (none to expert), purpose (personal vs. professional), frequency of use, how much they iterate, and whether the output must be shared with others.

**Three mutually exclusive segments:**

| Segment | Description | Reach | Underserved degree |
|---|---|---|---|
| Non-technical makers | Professionals and hobbyists with no coding background who want a small custom tool or page (budget trackers, event pages, planners) | High and growing | High: they hit a wall the moment something breaks or needs to persist, and can't debug |
| Technical prototypers | Developers and PMs who use Artifacts to test ideas fast, then move to a real codebase | Medium | Low-Medium: they have IDEs, Claude Code, and other tools |
| Document/knowledge workers | People producing reports, memos and plans with Claude, needing polish and collaboration | High | Medium: decent options exist (Docs, Notion, Word) |

**Mutual exclusivity check:** motivation separates them: tool-building without code, prototyping to ship, versus producing written work. A person might do more than one, but their primary job-to-be-done differs, and each needs substantially different solutions.

"I'll prioritize non-technical makers: high reach, highly underserved, and a perfect fit with the mission of empowering anyone. They're also a growth engine, since each shared creation introduces new people to Claude."

**Persona:** Priya, 34, operations manager at a mid-size logistics company. She has no coding background. She uses Claude daily for emails and analysis, and recently asked it to build a shift-swap tracker for her team. She's thrilled it appeared in seconds, but she's not a developer and can't tell why things sometimes break.

### Step 3: Problem identification

**Priya's journey, built around her shift-swap tracker:**
1. Spark: Realizes a spreadsheet isn't cutting it for her team's shift swaps.
2. Prompting: Describes what she wants; unsure how detailed to be.
3. First result: Claude generates a working tracker. Delight.
4. Refinement: She asks for tweaks (colors, a new column, approval status). Some edits break something else.
5. Real use: She wants her team of 12 to use it daily and see the same data.
6. Sharing and maintenance: Sends a link, edits later, wonders who can see what, tries to recover a previous version.

**Three problems:**
1. **Fragile iteration.** Priya struggles to make safe changes because each edit can silently break something that worked, so she loses trust and time and starts over. Frequency: high, every session. Severity: medium-high.
2. **Prototype-to-real-use gap.** Priya struggles to turn her artifact into something her team can rely on, because data doesn't persist or sync across users and she can't tell what's possible, so the tool stays a demo. Frequency: medium (happens when she tries to deploy). Severity: very high; it blocks the entire value.
3. **Opaque state and versions.** Priya struggles to understand what changed and to go back, because there is no clear change history or visual diff, which creates anxiety about experimenting. Frequency: high. Severity: medium.

"Scoring severity and frequency, I'll prioritize the prototype-to-real-use gap. Its severity is the highest, and it is the exact moment where Claude either becomes an indispensable work tool or stays a toy. It directly serves our mission: a working, shareable creation, not a demo."

### Step 4: Solution development

**Three distinct solutions to the prototype-to-real-use gap:**
1. **"Make it real" guided publishing.** Claude detects when an artifact needs persistence, multiple users or sharing, then walks the user through it conversationally ("Your team will need to see the same data. Want me to set up shared storage and publish a link?"), handling the plumbing behind the scenes.
2. **Template gallery of proven, team-ready artifacts.** Curated, pre-tested starters (trackers, forms, dashboards) that already include shared data and permissions, which Claude customizes.
3. **Export to a managed workspace.** One-click handoff into a hosted environment or integration with tools like Slack, Google Workspace and Notion, so artifacts live where teams already work.

**Impact vs. effort:**

| Solution | Impact | Effort | Rationale |
|---|---|---|---|
| Guided publishing | High | Medium | Solves the root cause in the flow where the user already is; builds on existing sharing and storage capabilities |
| Template gallery | Medium | Low | Fast to ship, but limited to predefined use cases; doesn't help with custom ideas |
| Export to workspace | Medium-High | High | Many integrations, partner dependencies, and divides attention |

"I'll prioritize guided publishing: high impact, moderate effort. It meets users inside the conversation, uses Claude's strength in understanding intent, and is hard to copy because it combines model intelligence with Anthropic's own product surface. It also changes Priya's experience: from 'I built a cool demo' to 'my team uses this every day.'"

**V1 definition:**
- **Trigger:** When Claude detects shareable or multi-user intent (words like "my team", "everyone", "daily"), it offers a one-tap *Make it team-ready* prompt.
- **What v1 does:** Claude asks 2-3 plain-language questions (Who needs access? Should people edit or only view? Should data be saved between visits?), then configures shared data storage, generates a link, and shows a short checklist of what's now enabled.
- **Safety rails:** Automatic snapshot before every major edit with one-click restore (a minimal answer to problems 1 and 3), and clear indication of who can see the artifact.
- **Scope:** Start with trackers, forms and simple dashboards for small teams (up to about 25 people) on the paid plans. Out of scope for v1: enterprise SSO, complex permissions, and external databases.
- **Distribution:** In-product prompt inside the artifact panel, plus a Share menu entry; a follow-up nudge after the user returns to an artifact a second time.

**Success metrics:**
- Primary: percentage of artifacts that are shared and reopened by at least one other person within 14 days.
- Secondary: weekly returning creators; retention of creators at 30 days.
- Guardrails: rate of artifacts reported as broken after publishing; support contacts per publish; safety and abuse reports.

**Risks and mitigations:**
- **Privacy and safety.** Shared artifacts could expose sensitive data or be misused. Mitigation: private-by-default sharing, explicit confirmation of who can see it, content and abuse safeguards, and clear data-handling disclosure.
- **Reliability.** Auto-configured storage could fail or lose data, destroying trust. Mitigation: automatic snapshots, staged rollout, and an obvious "restore" path.
- **Low discovery.** Users may ignore the prompt. Mitigation: contextual triggers on intent words, and testing copy and placement via A/B experiments.

**Vision beyond v1:** Artifacts become living team tools: version history with natural-language changelogs ("Claude changed the approval column; undo?"), integrations with calendars and chat, and a community library where people can remix each other's creations.

### Closing (tie back to the mission)

"To summarize: Artifacts matter because they turn conversation into creation. I focused on non-technical makers like Priya, found that the biggest barrier is the leap from demo to real team use, and proposed guided publishing as v1, with snapshots as a safety net. Success looks like shared artifacts that other people actually come back to. That moves us toward our mission: anyone can turn an idea into a working, shareable creation. If we had more time, I'd talk about the experiment plan for the first launch."

## 10. A four-week practice plan

- **Week 1: Foundations.** Memorize the framework. Write your assumptions and game-plan template. Practice five openings per day.
- **Week 2: Section drills.** Daily 10-minute drills: mission statements (Mon), ecosystem + segments (Tue), journeys + problems (Wed), solution brainstorms (Thu), v1 + risks (Fri).
- **Week 3: Full mocks.** Do 2-3 timed 35-minute mocks per week, ideally recorded. Review for waypointing, check-ins, and time per section.
- **Week 4: Feedback and polish.** Mock with peers or an AI copilot, particularly Claude Projects loaded with this framework. Fix your weakest dimension. Repeat on unfamiliar products.

### Self-review checklist after each mock

- Did I state assumptions and a game plan?
- Did I check in at least three times?
- Was my mission statement specific and used later?
- Were my segments mutually exclusive, with a clear 2x2 reason?
- Did I describe problems as obstacles, not wants or solutions?
- Did I propose three truly different solutions?
- Did I define a small v1, metrics and risks?
- Did I finish on time with a closing that ties back to the mission?
