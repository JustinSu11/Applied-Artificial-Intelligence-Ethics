# AI Ethics: Terms Cheat Sheet

> Quick reference for review. Read the **Fast Recall**
> first (30 sec), then jump to any term.
> Each term: **What** (plain words), **Hook** (memory
> trick), **Example**.

**Status:** Week 1 -> 1.1, 1.2, 1.3a, 1.3b done.
Week 2 -> 2.2 (parts 1 and 2) done, 2.1 pending.

---

## Fast Recall (30 seconds)

**Floridi's 5 ethics risks** = **B**uffet, **P**aint,
**L**awyer, **T**rash, **S**kip

| Hook   | Term             | Tell-tale sign                   |
|--------|------------------|----------------------------------|
| Buffet | Ethics shopping  | Picks the rule that fits them    |
| Paint  | Bluewashing      | Big claim, little action         |
| Lawyer | Ethics lobbying  | "We self-regulate, no law needed"|
| Trash  | Ethics dumping   | Banned here, tested over there   |
| Skip   | Ethics shirking  | Skips ethics where payoff is low |

**Predictive policing: 4 breaches** =
Dirty data -> Loop -> Black box -> Gut bias

**5 course principles** =
Dignity & freedom - Justice & fairness -
Privacy & safety - Explainability & transparency -
Responsibility

**Ethics vs Governance** =
Ethics asks "What *should* AI do?"
Governance asks "How do we *make sure* it does?"

**3 levels of governance** = Society -> Institutions
-> Individuals (laws -> audits -> codes & design)

**Publication ladder** (soft -> hard):
Value (compass) -> Principle (goal) ->
Framework (blueprint) -> Guidance (how-to) ->
Requirements (must-dos) -> Checklist (ALTAI)

**Hard rules ladder:** Law (what) ->
Regulation (how to carry it out) ->
Technical standard (exact spec)

**Actors vs Stakeholders** = actors *do* (build/run AI),
stakeholders are *involved or affected*.
Actors are a subset of stakeholders.

---

## Index (A-Z)

| Term                       | Lecture |
|----------------------------|---------|
| AI actors                  | 1.3a    |
| AI ethics vs AI governance | 1.3a    |
| Algorithmic audit          | 1.3a    |
| Assessment List (ALTAI)    | 1.3b    |
| Biased data                | 1.1     |
| Bluewashing                | 1.2     |
| CCPA                       | 1.2     |
| Confirmation bias          | 1.1     |
| Double standard            | 1.2     |
| EU AI Act                  | 1.3b    |
| Ethics by design           | 1.3a    |
| Ethics dumping             | 1.2     |
| Ethics lobbying            | 1.2     |
| Ethics shirking            | 1.2     |
| Ethics shopping            | 1.2     |
| Ethics washing (umbrella)  | 1.2     |
| Feedback loop              | 1.1     |
| Five principles            | 1.1     |
| Foresight & oversight      | 1.1     |
| Framework                  | 1.3b    |
| GDPR                       | 1.2     |
| Garbage in, garbage out    | 1.1     |
| Governance (3 levels)      | 1.3a    |
| Greenwashing               | 1.2     |
| Guidance (vs guidelines)   | 1.3b    |
| Impact assessment          | 1.3a    |
| Lack of transparency       | 1.1     |
| Law                        | 1.3b    |
| Not value neutral          | 1.3a    |
| Partnership on AI (PAI)    | 1.3a    |
| Personal values (compass)  | 1.2     |
| Predictive policing        | 1.1     |
| Principle                  | 1.3b    |
| Proxy attribute            | 1.1     |
| Regulation                 | 1.3b    |
| Requirements               | 1.3b    |
| Scientific veneer          | 1.1     |
| Self-regulation            | 1.2     |
| Stakeholders               | 1.3a    |
| Technical standard         | 1.3b    |
| Technical vs non-technical | 1.3a    |
| Unconscious bias           | 1.1     |
| Value                      | 1.3b    |
| AI impact assessment (AI-IA) | 2.2 p1 |
| Ethics impact assessment (EIA) | 2.2 p1 |
| IEEE 7010                  | 2.2 p1  |
| Intended user              | 2.2 p2  |
| Taxonomy                   | 2.2 p1  |
| Unintended user            | 2.2 p2  |
| Well-being impact assessment (WIA) | 2.2 p2 |
| Well-being indicators dashboard | 2.2 p2 |
| Stakeholder (IEEE 7010)    | 2.2 p2  |
| Stakeholder tiers          | 2.2 p2  |
| 4 impact dimensions        | 2.2 p2  |

---

# Week 1

## Lecture 1.1: The Power and Promise of AI

**Big idea:** AI can do huge good, but the outcome
depends on *how it's built* and *how it's used*.
Good intentions are not enough.

### Garbage In, Garbage Out (GIGO)
**What:** Bad data in = bad results out. (George Fuechsel)
**Hook:** A great chef can't fix rotten ingredients.
**Example:** Model trained on biased police records
gives biased predictions.

### Foresight & oversight
**What:** Think ahead about misuse, then keep watching
after launch.
**Hook:** What seems good today can be abused tomorrow.
**Example:** A tool built to help police gets used to
over-target neighborhoods.

### Predictive policing
**What:** Using data + predictive analytics to guess
where crime may happen (or who may offend).
**Hook:** Good intent, bad outcome.
**Example:** PredPol (now Geolitica) used by about 1/3
of US agencies by 2017.

### Biased data  *(breach 1)*
**What:** Past data reflects past human bias, and the
model copies it.
**Hook:** Dirty data in -> dirty decisions out.
**Example:** Over-policed area = more recorded crime
= model says "send more police," whatever the real
crime rate.

### Feedback loop (vicious)  *(core idea)*
**What:** Model output changes the real world, which
creates new data that feeds the model again.
**Hook:** A snake eating its own tail.
**Example:** Predict crime here -> patrol here ->
arrests here -> data says "crime here."

### Confirmation bias  *(breach 2)*
**What:** Seeing only evidence that confirms what you
already believe. Here, the system confirms itself.
**Hook:** Lawyer, not judge.
**Example:** More patrols find more minor offenses,
which "prove" the zone is high crime.

### Lack of transparency & accountability  *(breach 3)*
**What:** You can't inspect or challenge the model,
so nobody is answerable for bias.
**Hook:** Black box = no blame.
**Example:** Proprietary software, so outsiders can't
audit the algorithm.

### Unconscious bias  *(breach 4)*
**What:** Hidden biases of builders and users shape
design, rollout, and results.
**Hook:** Bias you don't know you have.
**Example:** Builders never asked how the data was
collected or what era it came from.

### Proxy attribute
**What:** A harmless-looking feature that stands in
for a protected trait.
**Hook:** A mask for race.
**Example:** Zip code or school attended, used by
Chicago's model to label people "high risk."

### Scientific veneer (for racism)
**What:** Math/AI makes biased results look
objective and neutral.
**Hook:** Racism in a lab coat.
**Example:** 1,400 mathematicians signed a 2020 letter
refusing to work with police on this.

### Five ethical principles (course roadmap)
1. Dignity & freedom
2. Justice & fairness
3. Privacy & safety
4. Explainability & transparency
5. Responsibility

**Hook:** every breach above maps to one of these.

### Case timeline: predictive policing
- **1930:** first uniform police report (Jim Crow era
  data later feeds models)
- **2008:** recession -> police budget cuts
- **2009:** first predictive policing symposium;
  LAPD gets $3M for trials
- **2012:** PredPol created
- **2017:** ~1/3 of agencies use predictive software
- **2020:** Chicago scraps program (85% of top-risk
  scores were African American men, many with no
  record); LAPD ends it; Santa Cruz first US city
  ban
- **May 2023:** European Parliament votes to ban it
  (still in use in the US)

---

## Lecture 1.2: Floridi, Ethics Washing

**Big idea:** Stop only debating *what* the standards
are. Start *doing* them. Floridi names 5 ways
companies fake it.

### Ethics washing (umbrella)
**What:** Looking more ethical than you are. The
5 risks below are its flavors.
**Hook:** Costume, not conduct.

### Ethics shopping  (Buffet)
**What:** Picking or bending ethical guidelines to
justify what you already do, instead of changing
behavior.
**Hook:** Ethics buffet: take only what you like.
**Example:** After GDPR (2018), Facebook gave EU users
strong privacy but moved ~1.5B non-EU users under
looser US-style terms.
**Result:** Inconsistent standards, weak accountability.

### Bluewashing  (Paint)
**What:** Misleading claims or shallow actions to look
digitally ethical without real change.
**Hook:** A fresh coat of paint over a cracked wall.
**Example:** Facebook in Myanmar: impact assessment
skipped the Rohingya communities, promises were
reactive and aimed at public perception.
**Tell:** Underfunded or powerless ethics councils.

### Greenwashing  *(the cousin)*
**What:** Same trick for the environment: seeming
greener than you are. Bluewashing = digital version.

### Ethics lobbying  (Lawyer)
**What:** Using "ethics" arguments to delay, weaken,
or avoid good laws.
**Hook:** Hire a lawyer to dodge the rules.
**Example:** Google and allies lobbied to soften the
CCPA, saying voluntary privacy measures were enough.
**Result:** Harmful practices stay unregulated longer.

### Self-regulation
**What:** "We police ourselves, no law needed."
**Hook:** The favorite excuse in ethics lobbying.

### Ethics dumping  (Trash)
**What:** Exporting practices to places with weak laws
that would be unacceptable at home (or importing the
results).
**Hook:** Taking your trash to someone else's yard.
**Example:** Huawei/ZTE smart cities in Africa: facial
recognition and surveillance with little oversight.
**Tell:** *Double standard*: strict where regulated,
loose where not. Locals become a **testing ground**.

### Ethics shirking  (Skip)
**What:** Doing less ethical work where the payoff
looks low.
**Hook:** Skipping the homework nobody grades.
**Example:** PredPol knew data was biased and the
feedback loop existed, but did little to fix it.
**Result:** Inequality, hits vulnerable groups most.

### Personal values (the compass)
**What:** Rules and company policy aren't enough.
Your own values guide you when no one is checking.
**Hook:** Compass, not rulebook.

### Supporting terms
- **GDPR:** EU privacy law (2018), very strict.
- **CCPA:** California law giving consumers control
  over their data (know, opt out of sale).
- **Double standard:** different ethics by region.
- **Testing ground:** weak-law region used to refine
  tech before bringing it to strict markets.

---

## Lecture 1.3a: Values & Intent of AI Ethics, Frameworks

**Big idea:** Ethics says what AI *should* do.
Governance makes it happen. And who writes the rules
matters, because rules are not neutral.

### AI ethics vs AI governance
**What:** Ethics = "What should AI do?"
Governance = "How do we ensure it does?" Policy-driven,
ideally with enforcement.
**Hook:** Ethics is the *goal*, governance is the *referee*.

### Technical vs non-technical governance
**What:** Two streams.
- *Technical:* make the system itself accountable
  (design justification, ethics by design, testing,
  validation).
- *Non-technical:* regulation, codes of conduct,
  certification, education, stakeholder input.
**Hook:** Fix the machine vs. fix the rules around it.

### Governance: 3 levels
1. **Society:** national/international law and human
   rights (e.g., Universal Declaration of Human Rights).
2. **Institutions:** guidance for orgs: risk management,
   impact assessments, audits, due diligence, CSR.
3. **Individuals:** ethics frameworks and professional
   codes (ACM, BCS, ISO, IEEE) plus design methods.

**Hook:** Big (laws) -> Medium (company process) ->
Small (your own work).

### Impact assessment
**What:** Check a system's effects *before* deploying.
Types: privacy, data protection, ethics, social,
human rights.
**Hook:** Look before you launch.

### Algorithmic audit
**What:** Independent check of an algorithm's behavior
and bias. An institution-level tool.

### Ethics by design (also: privacy by design)
**What:** Build ethics into the design process from the
start instead of bolting it on later.
**Hook:** Seatbelts installed at the factory.

### AI actors vs stakeholders (NIST)
**What:** *Actors* play an active role in the AI
lifecycle (build, deploy, operate). *Stakeholders* are
everyone involved or affected, directly or indirectly.
**Hook:** Actors act. Stakeholders are all who are
touched. Actors <= stakeholders.
**Actor types:** private sector, government,
international orgs, multi-stakeholder orgs, civil
society, natural persons.

### Not value neutral
**What:** Ethics and governance documents carry the
interests of whoever wrote them. They may or may not
serve the public good.
**Hook:** Always ask "who wrote this, and what do
they gain?"
**Link:** this is where ethics washing (1.2) lives.

### Partnership on AI (PAI)
**What:** Multi-stakeholder group: Apple, Amazon,
DeepMind, Google, Facebook, IBM, Microsoft. Also works
on the AI Incident Database.

### Actor roles (one-line summary)
- Natural persons: use AI and are affected by it
- Governments: rights, laws, regulations, standards
- Nonprofits: improve society in varied ways
- International orgs: help countries cooperate
- Corporations: build and deploy AI for profit
- Multi-stakeholders: alliances forming technical
  agreements, often for industry advantage

---

## Lecture 1.3b: Publications & Communications of AI Ethics

**Big idea:** AI governance runs on public documents
meant to shape behavior. They form a progression, and
each word means something different.
(You probably won't read these as a dev. Know the map.)

### The ladder (soft -> concrete)
**Compass -> Goal -> Blueprint -> How-to -> Must-dos
-> Checklist**
= Value -> Principle -> Framework -> Guidance ->
Requirements -> Assessment list

### Value
**What:** A conception of the desirable that steers
choices. The moral compass.

### Principle
**What:** High-level desirable goal for ethical conduct.
Context-free on purpose.
**Example:** EU Ethics Guidelines for Trustworthy AI:
respect for human dignity, freedom, democracy, justice
and rule of law, equality and non-discrimination,
citizen rights.

### Framework
**What:** Structured model outlining core values,
principles, and how they relate. The roadmap that
guides decisions.
**Hook:** The blueprint, not the building.
**Note:** Used in practice when laws/standards are
missing.

### Guidance (not the same as guidelines)
**What:** Practical recommendations for *how to apply*
a framework's principles. Companion to a framework.
**Hook:** The how-to manual.

### Requirements
**What:** Concrete, measurable criteria derived from
principles: what an AI system must do or avoid.
Written for designers, developers, deployers.
**Hook:** Sub-bullets under a principle you can
actually test.

### Assessment List (ALTAI)
**What:** EU Assessment List for Trustworthy AI. Turns
the requirements into a checklist for developers,
operators, deployers.
**Hook:** The to-do list at the end of the ladder.

### EU AI Act
**What:** Binding law that grew out of the EU's
human-rights-based framework. Includes risk
assessments and requirements.
**Hook:** Soft rules that hardened into law.

### Law / Regulation / Technical standard
- **Law:** rule made by government to order society.
- **Regulation:** official rule with detailed
  instructions on *how to carry out* laws.
- **Technical standard:** accepted protocol or spec
  (like a unit of measure) for an industry.
**Hook:** Law = what. Regulation = how.
Standard = exact spec.

### Who values what (compare lists)
- **Governments:** protect human rights, democracy.
- **Companies:** profit, innovation, efficiency.
- **EU principles:** human autonomy, prevention of
  harm, fairness.
- **OECD / GPAI:** inclusive growth, sustainable
  development, well-being come first.

**Questions to ask (from the lecture):**
- Is well-being the same as human rights?
- Is sustainable development the same as caring for
  the environment?
- "Inclusive growth": who is included?

---

# Week 2

## Lecture 2.1: (waiting for the correct transcript)

## Lecture 2.2: Helsinki AV Scenario and IEEE 7010

**Big idea:** impact assessments and standards are not
neutral. IEEE 7010 gives a process to assess a system's
effect on human well-being.

### Taxonomy
**What:** a **closed list of acceptable terms arranged
hierarchically** to describe and classify content.
Glossaries and definitions also classify.
**Warning:** taxonomies operationalize certain values,
can prioritize some stakeholders, and **miss true harms.**

### AI impact assessment (AI-IA)
**What:** identify **positive and negative impacts
early** to safeguard benefits and avoid downsides.
Can be self-assessments used for audits and legal or
standards requirements.
**Covers:** human rights, ethics, data protection,
privacy, security, safety, environment.
**Fits in:** organizational processes and the wider
governance system. **Not neutral.**

### Ethics impact assessment (EIA)
**What:** impact assessment focused on ethics. Like
AI-IAs and standards, **not neutral.**

### IEEE 7010
**What:** *Recommended Practice for Assessing the Impact
of Autonomous and Intelligent Systems on Human
Well-Being.* Produces a well-being indicators dashboard.

### Well-being impact assessment (WIA)
**What:** the IEEE 7010 process. **Iterative**, done at
**every phase** (concept, design, development,
ongoing monitoring). **5 activities:** internal
analysis, user/stakeholder engagement, indicators
dashboard, data collection process and collection, data
analysis and iteration.
**WIA activity one:** internal user and stakeholder
impact assessment (guidance pp. 21-22, Annex E).

### Well-being indicators dashboard
**What:** the output of the WIA, used to design, deploy,
monitor, and improve the system. At least **one
indicator per domain**, aligned with established datasets
(e.g., the World Happiness Report).

### Intended / unintended user / stakeholder
- **Intended user:** person the creator intends to use
  the system.
- **Unintended user:** not intended, but interacts with
  it anyway (children, tourists, suspended-license
  drivers).
- **Stakeholder:** anyone meaningfully (or potentially)
  **impacted by** the system **or impacting it** (police,
  insurers, data labelers, pedestrians).

### Stakeholder tiers (Helsinki pilot)
1. Directly impacted
2. Elderly and vulnerable populations
3. Indirect and future users and stakeholders

### 4 dimensions of an impact assessment
**Stakeholders, harms, risk, values.**

### Case: Helsinki AV pilot
Goal: end personal car ownership by 2040. Pilot on an
island, ~5,000 people, one month. Providers: INVIDA
(AI), Cargle (cars), SimTech (infrastructure). Uses
**"satisfaction with life"** as an indicator.

---

## Next lecture: (waiting for transcript)
