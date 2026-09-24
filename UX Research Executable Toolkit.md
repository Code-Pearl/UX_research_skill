# UX Research Executable Toolkit
### Extracted and operationalized from *Think Like a UX Researcher* (Travis & Hodgson, CRC Press 2019)

This is a hand-off document. Give it to a person or an AI and they can run a full UX research project end to end. Each framework below is self-contained and has four parts:

- **WHEN** — the trigger condition for using it
- **INPUTS** — what you need before starting
- **STEPS** — the exact procedure to execute
- **OUTPUT** — the artifact it produces
- **EXAMPLE** — a fully worked instance so the executor knows what "done" looks like

The frameworks are ordered in the sequence a real project runs: **Frame → Plan → Recruit → Conduct → Analyze → Act → Improve**. Run them top to bottom. Skip a block only when its WHEN condition is not met.

***

## The One Governing Principle (read first)

Everything in this toolkit rests on a single rule of thumb: **behavioral data is strong, opinion data is weak**. UX research is about observing what people *do*, not canvassing what they *say* or *like*; opinions are not evidence because for every 10 people who like a design, 10 will hate it and 10 won't care. Before collecting any data, the executor must always ask: *"What kind of data must I collect to provide credible evidence on this issue?"* — and let the method follow from that, never the reverse (never "we need a survey, let's do a survey").[^1]

**Strength-of-evidence ladder** (use this to choose or defend any method):[^1]

| Strength | Methods | Why |
|---|---|---|
| **Strong** | Field visits/contextual research, formative & summative usability tests, web/search analytics, A/B & multivariate tests, controlled experiments, task analysis | Users doing real tasks; objective, observable, replicable behavior[^1] |
| **Moderate** | Heuristic evaluations, cognitive walkthroughs, expert reviews (with real tasks), interviews, jobs-to-be-done, journey mapping, diary studies, card sorting, eye tracking, guerrilla research | Includes tasks or self-reported behavior, but higher variability[^1] |
| **Weak (avoid)** | "Which design do you like best?" tests, interview-only data collection, unmoderated "act like a reviewer" tests, focus groups, surveys as primary data, intuition, opinions of colleagues/boss | Guesswork or opinion; no place in UX research[^1] |

***

# PHASE 1 — FRAME THE PROBLEM

## Framework 1.1 — The Two-Question Method Selector

**WHEN:** At the very start of any project, to decide what type of research you even need.

**INPUTS:** A rough problem statement and knowledge of where you are in the development lifecycle.

**STEPS:**
1. Ask the two fundamental questions all UX research answers:
   - (a) *Who are our users and what are they trying to do?* → answered by a **field visit**.
   - (b) *Can people use the thing we've designed to solve their problem?* → answered by a **usability test**.
2. Map to lifecycle: if in **discovery** and unsure a real problem exists, run **field research** ("turn on the lights"). If later, with a design/prototype to evaluate, run a **usability test** ("look under the microscope").
3. Decision test: *Is there a user problem to be solved?* If unsure → field research. *Have we solved it?* If unsure → usability test.

**OUTPUT:** A one-line decision: "This project needs [field research / usability testing / both] because [validating the problem / validating the solution]."

**EXAMPLE:** A team wants to build a parcel-delivery app. They cannot cite evidence anyone struggles with current delivery. → Decision: *"Run field research first to validate the problem hypothesis (is delivery actually a painful problem?), then usability-test the prototype later to validate the solution hypothesis."*

***

## Framework 1.2 — Anatomy of a Research Question

**WHEN:** Before any study, to replace vague objectives ("get some insights," "hear the voice of the customer") with a real question.

**INPUTS:** The problem area and stakeholder goals.

**STEPS:**
1. Write ONE underlying question that guides the whole study. It is *not* a question you ask a participant — it's the driving force behind the investigation (e.g., "Does drinking coffee affect employee productivity?" not "Do you like coffee?").
2. Check it against all six criteria — a good research question must:
   - Be interesting
   - Ask something important
   - Be focused and specific
   - Lead to a testable hypothesis
   - Allow predictions based on measurable data
   - Advance the company's knowledge beyond the obvious
3. If it fails any criterion, rewrite it.

**OUTPUT:** A single sentence ending in a question mark that you could write on a whiteboard.

**EXAMPLE:** Weak objective: *"We want to understand our checkout."* → Strong research question: *"What causes first-time buyers to abandon the checkout before entering payment details?"* — specific, important, measurable (abandonment rate), and testable.

***

## Framework 1.3 — The "19 Days to Define a Problem" Four Techniques

**WHEN:** The brief is weak or you have time to sharpen the problem before committing to a method.

**INPUTS:** Initial brief/RFP, access to stakeholders.

**STEPS (apply all four):**
1. **Find out what other stakeholders need to know.** List all stakeholders (marketers, engineers, designers, support agents, tech writers, business analysts, legal). Meet each. Ask: what do they know about the problem, what's been tried, what happens if nothing is done, why this, why now, what does success look like, what are the constraints, timeline, budget.
2. **Deconstruct the construct.** Most things you study (usability, quality, satisfaction) are *constructs* — they can't be directly observed. Break them into measurable sub-components. Read the literature first; don't guess the components.
3. **Measure something.** Ask: what specifically must I measure? What metrics differentiate concepts? What's the dependent variable? What must I control? Will this convince the team? Can I use objective behavioral measures instead of rating scales?
4. **Shake out the issues.** Run a cheap **pre-pilot** ("hitting the grass to startle the snake") — air the problem in front of a few users with no lab/equipment to flush out hidden issues and missed stakeholders before committing budget.

**OUTPUT:** A refined problem statement, a stakeholder needs list, a set of measurable sub-components, and a list of surfaced risks.

**EXAMPLE:** Construct = "quality" of a product. Deconstructed into measurable sub-components: performance, features, reliability, conformance to standards, durability, serviceability, aesthetics. "Usability" deconstructs (per ISO 9241-11) into **effectiveness, efficiency, and satisfaction** — now each is separately measurable.

***

## Framework 1.4 — Desk Research (Secondary Research) via the Venn Method

**WHEN:** Before any primary research, to avoid re-discovering what's already known.

**INPUTS:** The product domain, access to internal reports/analytics/stakeholders.

**STEPS:**
1. Model the context of use as three overlapping circles: **Users**, **Goals**, **Environments**. The sweet spot is where all three overlap (field visits of your users pursuing their goals in context) — rare and precious.
2. Search the three two-way overlaps: (a) users+goals not in context (surveys, interviews, focus groups); (b) goals+environment but not users (call-center/web analytics); (c) users+environment but not goals (field research by teams building different products for the same users).
3. Mine internally first — talk to stakeholders/product owner, examine call-center and web analytics, talk to front-line customer-facing staff.
4. Then search each single circle for generic research on your users, your goals, your environments.

**OUTPUT:** A short synthesis of prior findings and open gaps, so you "know when you've discovered something new".

**EXAMPLE:** Building a genealogy app. No direct study exists, but desk research finds: internal search logs showing top queries (goals+environment), a marketing survey of hobbyist demographics (users+goals), and an academic ethnography of how retirees use tablets (users+environment). Together they frame the primary study.

***

# PHASE 2 — PLAN & SELECT USERS

## Framework 2.1 — The 2×2 User-Group Prioritization Grid

**WHEN:** The team says "our product is for everyone," or you don't know which users to research first.

**INPUTS:** The development team, sticky notes.

**STEPS:**
1. Give each team member sticky notes; working alone, each writes ≥5 candidate user groups (one per sticky). Prompt with: typical users, their opposite, early adopters, power users, who'd struggle, who'd only use it if forced, who's easiest to reach.
2. Remove duplicates.
3. Plot every group on a grid: vertical axis = **"Amount we expect to learn from this group"** (a lot / a little); horizontal axis = **"Ease of access"** (harder / easier).
4. Label quadrants: **Gold** = high-learning + easy-access (start here, sessions within days); **Silver** = high-learning + hard-access (add to backlog, plan now); **Bronze** = low-learning + easy-access (do only after gold/silver); low-learning + hard-access = **skip entirely, guilt-free**.

**OUTPUT:** A prioritized, gold/silver/bronze user-group list — a pragmatic starting point.

**EXAMPLE:** A photography app generates groups: day-trippers, food enthusiasts, Instagrammers, professional wedding photographers (abroad, hard to reach). Instagrammers = Gold (easy, high learning) → start there; wedding pros = Silver → backlog.

***

## Framework 2.2 — The Perfect Participant Screener (8 Rules)

**WHEN:** Recruiting anyone for a study — get representative, articulate participants and avoid no-shows.

**INPUTS:** Behavioral profile of target users, recruiting channel/agency.

**STEPS — apply all eight rules:**
1. **Screen for behaviors, not demographics** — past behavior predicts performance far better than gender/income. On web projects use two behavioral variables: **digital skills** and **task/domain knowledge**, classifying each candidate high/low on both.
2. **Ask precise questions** — not "how long online?" but "what do you do online, and alone or with help?" (buy with a credit card, install software, manage privacy, etc.).
3. **Identify unsuitable candidates early** — build the screener as a funnel: exclusion questions first. Avoid "faking good": ask open questions ("Where do you work?") instead of listing competitor companies.
4. **Get value-for-money participants** — for think-aloud, screen out shy/inarticulate people via an open question; for eye-tracking, exclude bifocals/rimless glasses/heavy mascara.
5. **Manage expectations** — clarify the screener isn't the study; incentive paid in cash on attendance; mention recording, consent form, NDA; interviewed alone (not a focus group). Don't reveal the specific product (prevents prepping).
6. **Pilot-test the screener** — run on people you know you want and don't want; confirm they sort correctly; get stakeholder sign-off so they can't later dismiss the sample.
7. **Avoid no-shows** — emphasize the participant's importance, send letter + email + map, give a phone number, use a named sender, confirm the day before, text on the day. Consider **floaters** (paid stand-bys) and **double-recruiting** for critical slots.
8. **Brief the recruiting company** — walk through the screener with the *actual* recruiter, flag ambiguities, mark where flexibility is allowed.

**OUTPUT:** A tested screener questionnaire + a recruited, confirmed participant roster.

**EXAMPLE:** Testing an eyeglasses e-commerce site. Screener funnels out competitor employees (open "where do you work?"), classifies digital skills high/low, and — after a real test failed because a participant deferred purchase decisions to his partner — adds a rule: recruit only people who make their own purchase decisions.

***

# PHASE 3 — CONDUCT THE RESEARCH

## Framework 3.1 — Field Visit / Contextual Research

**WHEN:** Answering "who are our users and what are they trying to do?" — discovery phase.

**INPUTS:** Recruited users in their real environment (home/workplace), research question.

**STEPS:**
1. Go where the action happens (home or workplace), not a lab — "get out of the building," but do a real visit, not a coffee-shop chat (the "safari, not the zoo" principle: observe natural behavior in the natural environment).
2. Observe real behavior — what people *do*, not just what they say.
3. Capture the full context: workflow across channels, needs, goals, pain points; and the six things your models must record — primary goals, task workflow, mental models, tools used, environments, and the terminology people use.
4. Use it to **validate the problem hypothesis**: is this really a problem, and how serious? (an "itch" people won't pay to scratch is not a viable problem).

**OUTPUT:** Field notes and observations feeding personas, journey maps, and task models.

**EXAMPLE:** A delivery-route app. Field visit reveals a driver "plans his route around lunch so he's near a bakery at noon" — a real goal invisible from a lab, and a design opportunity.

***

## Framework 3.2 — Writing Test Tasks (not questions)

**WHEN:** Preparing a usability test.[^1]

**INPUTS:** Top user tasks (ideally from field research or a top-tasks survey).

**STEPS:**
1. Remember: *there are no questions in usability — you write a list of tasks, not questions*. You're finding out if people *can use* it, not if they *like* it.[^1]
2. Turn the top handful of user-rated tasks into realistic scenarios.
3. Don't hand participants a task whose wording gives away the solution; for "scavenger-hunt" style tasks, be specific about the goal without revealing the path.
4. For troubleshooting scenarios, recreate the real issue and start the user at a search engine or help page to see their real terminology.

**OUTPUT:** A task list / scenario set for the moderated session.

**EXAMPLE:** Instead of asking "Do you find booking easy?", give the task: *"You need a suitcase no larger than 55×40×20 cm for a cabin bag. Find one and add it to your basket."* — realistic, measurable, not leading.

***

## Framework 3.3 — Moderating a Usability Test: The Five Mistakes to Avoid

**WHEN:** Running any moderated usability session.

**INPUTS:** Participant, tasks, recording setup.

**STEPS — actively avoid all five mistakes:**
1. **Talking too much** → *Embrace the silence.* Keep the intro to ~5 minutes. Ask the participant to do the task, then shut up, observe, listen. If you must speak, use only one stock phrase: *"Tell me more about that."*
2. **Explaining the design** → Never say "what the developers meant was…" You'll bias behavior and be seen as defending the product. Instead say: *"Tell me what you're doing right now."* Save any explanation for after the session.
3. **Answering questions** → Participant questions are "gold dust" because they signal a problem; the gold is in watching them solve it. Use the **boomerang technique**: answer a question with a question ("How do you think you'd get back to the beginning?").
4. **Interviewing rather than testing** → During tasks you are an *observer*. Sit behind and to one side; avoid eye contact; run a **pre-test interview** (background) and a **post-test interview** (overall assessment + the team's shopping-list questions) — but keep the task time pure observation.
5. **Soliciting opinions/preferences** → Don't ask which design they prefer or if they like a feature. Usability testing is about what *works best*, not what they *like*.

**OUTPUT:** A clean set of behavioral observations with minimal moderator bias.

**EXAMPLE:** Participant asks "Where's the shipping cost?" Novice moderator points to it (mistake #3). Correct move: *"Where would you look for it?"* — then observe where they actually search, revealing whether it's a critical or minor problem.

***

## Framework 3.4 — Usability Expert Review (avoiding personal opinion)

**WHEN:** You need efficient problem-finding without recruiting users, or as a precursor to testing.

**INPUTS:** The interface, a data-driven description of users and their tasks, 3–5 reviewers.

**STEPS — fix the four classic problems:**
1. **Take the user's perspective, not yours** — "it doesn't matter what you like." Start with a data-driven description of users and tasks so you can *predict* where users look, what they need, and where they'll click. If you can't describe users/tasks, test with real users instead.
2. **Use 3–5 reviewers, not one** — a single reviewer finds only ~60% of the issues a team of three finds; different reviewers catch different problem types (domain, visual, IA).
3. **Use technology-specific guidelines**, not generic principles alone.
4. **Judge which problems matter** — apply severity rating (see Framework 5.1) rather than listing everything flat.

**OUTPUT:** A consolidated, prioritized list of predicted usability problems.

**EXAMPLE:** Reviewing a banking app: three reviewers (one with finance domain knowledge, one visual-design-sensitive, one IA-sensitive) each begin by writing the target user's goals and tasks, then independently flag issues; results are merged and severity-rated.

***

## Framework 3.5 — Controlling Researcher (Experimenter) Bias

**WHEN:** Any study — bias favors the researcher's hypothesis ~70% of the time.

**INPUTS:** The study protocol, data loggers.

**STEPS:**
1. Understand the gold standard is the **double-blind** (nobody moderating/observing/analyzing knows the hypothesis or which condition is which) — but it's nearly impossible in UX; approximate it where you can (e.g., blind data loggers, remote unmoderated tools).
2. **Interaction biases (Clever Hans):** stay neutral in tone, posture, expression; don't lean/nod toward the sponsor's design; don't use leading/loaded questions or reassurances; stay out of the participant's line of sight; leave the room during summative tasks if possible; video-record yourself and review for tells.
3. **Recording/interpreting biases:** decide the data-logging codes ahead of time; record objective data (completion rate, time on task); agree pass/fail criteria beforehand; use ≥2 data loggers for inter-scorer reliability; record verbatim, not interpretation; double-check coding/entry; have a colleague critique the final report.
4. **Sponsorship & confirmation bias:** "you should not care what the outcome is — only that your design and data are bulletproof." Let the chips fall; report negative findings straight.

**OUTPUT:** A bias-controlled protocol and a defensible dataset.

**EXAMPLE:** A moderator stayed neutral introducing competitor designs but "leaned forward and nodded" for the sponsor's design — a Clever Hans bias caught only by reviewing the session video.

***

# PHASE 4 — ANALYZE

## Framework 4.1 — Observations → Insights → Hypotheses → Design Solutions

**WHEN:** After a usability test, to convert raw observations into actionable fixes (a test finds problems, not solutions).

**INPUTS:** All raw observations, sticky notes, the development team, a whiteboard.

**STEPS:**
1. **Start with clean data.** An *observation* is an objective description of what you saw/heard (a direct quote, a user goal, a user action, a pain point, a surprise) — **never** an interpretation or a solution.
2. **Reduce.** Remove duplicate observations (but note how many participants hit each — for later prioritization); discard irrelevant factoids.
3. **Affinity-diagram.** Write each observation on a sticky; with the team, group them on a whiteboard into logical clusters. Rule of thumb: 100 observations → ~10–15 groups, not 100.
4. **Generate insights.** For each cluster write ONE insight as a provocative, point-of-view sentence — like a headline (e.g., *"Users don't use the same names for things as we do"*). Your job is to be the "grit in the oyster".
5. **Prioritize.** Dot-vote with the team; pick the **top 3** issues to fix; don't try to fix everything.
6. **Develop hypotheses.** For each top insight, list every plausible root cause (most insights have several); a gut feeling without data is just a gut feeling.
7. **Create design solutions.** Apply Krug's rule: *"What's the smallest, simplest change that's likely to keep people from having this problem?"* Each hypothesis maps to a different minimal tweak — testable in days, not a redesign taking months.

**OUTPUT:** Top-3 insights, each with candidate hypotheses and a minimal, testable design change.

**EXAMPLE:** Observation: users never tapped the vertical-ellipsis (⋮) "more actions" menu. Insight: *"Users don't recognize the ⋮ as a control."* Hypotheses: (a) they think it's branding, (b) it's too far right where people don't look, (c) they think it does something else, (d) they don't need it. Each yields a different small design change to A/B test next iteration.

***

## Framework 4.2 — Prioritizing Usability Problems: 3-Question Severity Decision Tree

**WHEN:** A test returns 100+ issues and the team needs to know what to fix first, defensibly.

**INPUTS:** The list of identified problems.

**STEPS — ask three questions per problem:**
1. **Impact:** Does it affect task completion (esp. frequent/critical tasks)? High-impact = worse than a satisfaction-only issue.
2. **Number affected:** Does it hit many users or just a few? Many = more severe.
3. **Persistence:** Does it recur throughout the interface (global vs. local)? Persistent = more severe.
4. Run the answers through the decision tree to assign a level, then interpret:
   - **Critical** — users can't/won't complete a common task → fix urgently.
   - **Serious** — significantly slows users or forces a workaround → fix ASAP.
   - **Medium** — frustrating but doesn't block completion → fix in next BAU update.
   - **Low** — cosmetic (e.g., a typo) → minor, but too many lows damage credibility/brand.

**OUTPUT:** Every problem tagged Critical/Serious/Medium/Low with a transparent, repeatable rationale.

**EXAMPLE:** A site with no underlined hyperlinks: high impact (users can't find links without "minesweeping"), many users, and persistent across every page → **Critical**.

***

## Framework 4.3 — The Baloney Detection Kit (10 Critical-Thinking Tools)

**WHEN:** Evaluating whether the team is building the *right* product / challenging shaky ideas at kick-off or stage gates (given ~90% of new products fail).

**INPUTS:** The idea, claim, or product mandate under scrutiny.

**STEPS — apply the ten tools (from Carl Sagan):**
1. **Confirm the facts** — require independent confirmation; trace secondary sources back to the original.
2. **Encourage debate** — substantive debate on the *evidence* by proponents of all views (not opinions).
3. **Authorities can be wrong** — "data beats opinion, no matter whose opinion it is"; don't pull rank, present data.
4. **Develop more than one idea** — generate multiple hypotheses/solutions, then try to *disprove* each; keep the one that survives.
5. **Keep an open mind / don't get attached** — be willing to pivot; being wrong is OK.
6. **Quantify** — attach numbers; vague/qualitative claims allow too many explanations.
7. **Test every link in the chain** — every premise and every product element must hold; use stage gates as checkpoints.
8. **Apply Occam's Razor** — of two equal explanations, choose the simpler; also design for simplicity to fight feature creep.
9. **Test the hypothesis (falsifiability)** — if it can't in principle be falsified, it's worth little; reject untestable questions like "how likely are you to buy this?"
10. **Conduct experiments** — decide among competing ideas with carefully designed, bias-controlled (ideally double-blind) experiments — the core of Lean UX.

**OUTPUT:** A go/no-go recommendation backed by evidence, with flawed assumptions exposed.

**EXAMPLE:** "We're building this because our competitor is." Apply tool #1/#3: *Why are they building it? What do they know that we don't? How do we know they got it right?* — forces evidence before committing budget.

***

# PHASE 5 — ACT ON THE FINDINGS

## Framework 5.1 — The Agile Persona (2D Sketch)

**WHEN:** You need a lightweight, updatable user model instead of a glossy, "cast-in-concrete" persona.

**INPUTS:** Completed UX research (you must have done the research — don't brainstorm personas from thin air), flip-chart paper, Sharpies, sticky notes, the team.

**STEPS:**
1. Reach a shared understanding of the research done so far; agree on the distinct user groups.
2. Turn flip-chart paper landscape; split into four quadrants.
3. Fill each quadrant, one item per sticky note:
   - **Top-left:** name for this user type + a sketch of them in context with a relevant thought.
   - **Bottom-left — Facts:** things known to be true (age, job title, gender).
   - **Top-right — Behaviors:** what they want to do / currently do related to the product.
   - **Bottom-right — Needs & Goals:** how they want to feel, deep motivations, what they ultimately want to achieve.
4. Prioritize stickies in each quadrant; have the conversation; reach shared understanding.
5. **Do not** polish it into a glossy artifact — post it on a wall and update it as you learn more; "it's the process that matters, not the beauty of the final artifact".

**OUTPUT:** A disposable, wall-mounted 2D sketch persona that serves as a conversation starter.

**EXAMPLE:** For a budgeting app: Name = "Freelancer Farah," Sketch = her at a café checking income. Facts: 34, self-employed designer. Behaviors: reconciles invoices weekly, dreads tax season. Needs/Goals: wants to feel in control and never be surprised by a tax bill.

***

## Framework 5.2 — Getting the Team to Take Action (Transition & Recommendations)

**WHEN:** After analysis, to ensure findings actually change the product.

**INPUTS:** Insights, prioritized problems, proposed solutions.

**STEPS:**
1. Run a **one-day research + design workshop** to explain what you found and how, and to transition findings and solutions to the team.
2. Provide **specific, actionable design recommendations** (you're a full member of the team, not just a critic — don't stop at "here are the observations").
3. **Agree accountability** for implementing each recommendation.
4. **Promote iterative design** — arrange to test multiple prototype versions.
5. Present a clear series of next steps (tactical + strategic); educate the team in UX methods; chair the design meetings, don't just attend.
6. Choose the right format to share findings for the audience: report, presentation, daily stand-up, or highlights video.

**OUTPUT:** An action plan with owners, next test dates, and agreed recommendations.

**EXAMPLE:** After a checkout study, hold a half-day workshop; hand the team three prioritized fixes each with a named owner and a commitment to re-test the revised prototype next sprint.

***

# PHASE 6 — IMPROVE YOUR OWN PRACTICE

## Framework 6.1 — Structured Reflection (with 5 Whys)

**WHEN:** Continuously — after each stage of a project (not just at the end).

**INPUTS:** A just-completed research activity; a log (Moleskine, e-notebook, template, or audio/video diary).

**STEPS — use this format:**
1. **What** activity did you do? (date, type, sample size, session length, total time.)
2. **Why** that activity rather than another?
3. **What went well?** Name 2–3 specifics.
4. **What went badly?** Name 2–3 specifics.
5. **Analyze** — for each good/bad point ask "Why?"; go deep using the **5 Whys** technique; avoid superficial reflection.
6. **Integrate** — how will you apply what went well elsewhere? When might it not work?
7. **Ask "What if?"** — how will you prevent the bad parts recurring? What will you do differently next time?

**OUTPUT:** A dated journal entry that feeds future portfolio case studies and skill growth.

**EXAMPLE:** After a session that ran long: What went badly = "3 tasks didn't fit in 60 min." 5 Whys → root cause = "the intro ran 15 min because I over-explained." Integrate → cap the intro at 5 min next time (ties directly to Mistake #1 in Framework 3.3).

***

## Framework 6.2 — The 8-Competence Star Chart (team/self assessment)

**WHEN:** Assessing or developing a UX practitioner/team.

**INPUTS:** The eight competences and a 0–5 scale.

**STEPS:**
1. Rate each of the eight competences on the 0–5 scale (0 = non-existent → 5 = expert, develops new applications):
   - User needs research · Usability evaluation · Information architecture · Interaction design · Visual design · Technical writing · UI prototyping · UX leadership.
2. Have people **self-assess** using concrete behavioral descriptors for each competence.
3. Counter the **Dunning-Kruger effect** (novices over-rate, experts under-rate): either ignore absolute scores and read the *pattern* across the eight, or follow up each chart with an interview demanding specific behavioral examples.
4. Plot as a star/radar chart to reveal the person's "signature," compare against role benchmarks, and target development.

**OUTPUT:** A competence signature per person; gaps to develop; behavioral criteria for hiring.

**EXAMPLE:** A "UX Researcher" role signature should show expertise (4–5) in **user needs research** and **usability evaluation**, with basic literacy across the other six.

***

## How the Frameworks Chain Together (one continuous run)

Hand this sequence to an executor as the master workflow:

1. **1.1** decide field visit vs. usability test → **1.2** write the research question → **1.3** sharpen the problem (stakeholders, deconstruct, measure, pre-pilot) → **1.4** desk research.
2. **2.1** pick gold user groups → **2.2** screen & recruit them.
3. **3.1** field visit (if validating the problem) → **3.2** write tasks → **3.3** moderate the usability test → **3.4** expert review (optional) → **3.5** control bias throughout.
4. **4.1** observations→insights→hypotheses→solutions → **4.2** severity-rate the problems → **4.3** apply the Baloney Detection Kit to go/no-go calls.
5. **5.1** build 2D-sketch personas → **5.2** run the transition workshop and secure action.
6. **6.1** reflect after each stage → **6.2** update competence signatures.

The connective tissue across all six phases is the governing principle: **collect behavioral evidence, prioritize by strength of evidence, and let the data — not opinion — decide**.[^1]
  <!-- by CODE__PEARL | this-is-maddness.com -->

---
