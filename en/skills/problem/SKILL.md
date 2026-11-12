---
description: "Apply the problem discovery and definition frameworks (9 types) interactively"
---

# Problem discovery and definition frameworks

Based on the user's $ARGUMENTS, apply the appropriate framework from the list below. If there is no argument, ask the user about their situation and propose one.

---

## 01. As-is/To-be
**Purpose**: Clarify the gap between the current state (As-is) and the ideal state (To-be), and define the issues to work on

**Template**:
| Item | As-is (current) | To-be (ideal) | Gap (difference) |
|------|-------------|-------------|-----------|
| Item 1 | | | |
| Item 2 | | | |
| Item 3 | | | |

**How to use**: First describe the ideal state in concrete terms, then write out the current state honestly. The difference between the two is the issue itself. Including quantitative metrics in the ideal state makes the gap clear. Describe the current state based on data and facts, without wishful thinking.

**Example** (improving monthly sales of an e-commerce site):
| Item | As-is (current) | To-be (ideal) | Gap (difference) |
|------|-------------|-------------|-----------|
| Monthly sales | 8 million yen | 15 million yen | +7 million yen (87.5% increase) |
| CVR | 1.2% | 2.5% | +1.3 pt |
| Average order value | 3,200 yen | 4,500 yen | +1,300 yen |
| Repeat rate | 15% | 35% | +20 pt |
| Cart abandonment rate | 72% | 45% | -27 pt |

**Common mistakes**:
- **Vague ideal**: Quantify it, such as "15 million yen per month" instead of "we want to increase sales". For items that cannot be quantified, describe a concrete "state" (example: "a state where inquiry handling does not depend on specific individuals")
- **Flattering the current state**: Out of habit from internal presentations, people make the current state look better than it is. Use data that a third party can verify
- **Leaving the gap as is**: Being satisfied once the gap is identified, and not moving on to prioritization or planning actions

**Tips**:
- Narrow the items down to 3 to 7. Too many items blur the focus
- State a deadline for the To-be (example: "as of the end of Q3 2025")
- The item with the largest gap is not always the one to start with. Judge priority by both feasibility and impact
- Include qualitative items (example: organizational culture, customer satisfaction) to keep balance

**Next steps**:
- Dig into the causes of the gap → use **Why-Why Analysis (5 Whys)** or the **Cause-and-Effect Diagram**
- Prioritize actions → organize with the **Urgency/Importance Matrix**
- Set the ideal based on the market environment → use **PEST Analysis** or **3C Analysis** in the `/market` skill
- Build a concrete strategy → move to the `/strategy` skill

---

## 02. 6W2H
**Purpose**: Break down an issue or plan from multiple angles and define it without gaps

**Template**:
- **What** (the object):
- **Why** (the reason):
- **Who** (the actor):
- **Whom** (the target):
- **When** (the timing):
- **Where** (the place):
- **How** (the method):
- **How much** (the cost):

**How to use**: Break a vague issue down through 8 lenses. You do not have to fill in everything; blank fields show where information is missing. This is especially useful when writing a proposal or launching a new project, to prevent misalignment among stakeholders.

**Example** (internal DX promotion project):
- **What** (the object): Migrate the sales department's customer management from Excel to a CRM (Salesforce)
- **Why** (the reason): Customer information depends on individuals, so handover is difficult when a person transfers or leaves. Sales activity is also not visible, so management relies on intuition
- **Who** (the actor): DX promotion office (leader: Tanaka) + 3 members selected from the sales department + 2 members from the IT department
- **Whom** (the target): All 50 members of the sales department are direct users. Executives view the dashboard
- **When** (the timing): April to September 2025 (6 months). Pilot operation starts in July in Sales Section 1
- **Where** (the place): Tokyo head office first, Osaka and Nagoya branches in phase 2
- **How** (the method): Introduce Salesforce Sales Cloud. Migrate existing Excel customer data via ETL. Hold weekly training for 2 months
- **How much** (the cost): Initial implementation 8 million yen + annual license 6 million yen. ROI target: recover the investment in 2 years

**Common mistakes**:
- **Confusing Why and What**: Distinguish "increase sales (What)" from "because market share is declining (Why)"
- **Missing Whom**: Proceeding while the target or beneficiary of the action is vague. In BtoB especially, separate the "decision maker" from the "user"
- **Underestimating How much**: Include not only direct costs but also labor costs, training costs and opportunity costs

**Tips**:
- Starting with Why keeps the project's essential purpose from drifting
- Mark items you cannot fill in as "areas that need research", and assign an owner and a deadline
- When there are multiple stakeholders, have each fill in the 6W2H separately to find gaps in understanding
- Update it regularly (for example monthly) to track divergence between plan and reality

**Next steps**:
- Structure the issues identified with 6W2H → break them down with the **Logic Tree**
- Make the project plan concrete → use the **WBS** or **Gantt Chart** in the `/execution` skill
- Dig into target customers → use **Persona** in the `/customer` skill
- Communication plan → use the `/communication` skill

---

## 03. Why-Why Analysis (5 Whys)
**Purpose**: Reach the root cause from a surface-level problem

**Template**:
```
Problem: _______________
Why 1: _______________
  Why 2: _______________
    Why 3: _______________
      Why 4: _______________
        Why 5: _______________
→ Root cause: _______________
→ Countermeasures: _______________
```

**How to use**: Repeat "why?" at least 5 times. If the chain branches along the way, combine it with a Logic Tree. Each answer must be based on facts. Proceeding on guesses leads to a wrong root cause.

**Example** (sales decline on an e-commerce site):
```
Problem: Last month's e-commerce site sales fell 20% compared to the previous month
Why 1: Because the number of completed purchases dropped sharply
  Why 2: Because the abandonment rate after adding to cart rose from 72% to 85%
    Why 3: Because errors occurred frequently on the payment screen
      Why 4: Because we had not handled the payment provider's API specification change
        Why 5: Because the person in charge missed the API change notification email, and no verification was done in the test environment
→ Root cause: There is no process to detect and respond to specification changes in external services
→ Countermeasures: (1) Set up a shared channel for external API change notifications (2) Introduce a monthly checklist of external service changes (3) Build regular automated tests in the staging environment
```

**Common mistakes**:
- **Stopping at "someone's fault"**: "Because the person in charge was negligent" is not a root cause. Dig down to structural and process problems: "Why does the system allow negligence?"
- **Leaps in causality**: Check every time that there is no logical leap between "Why 1 → Why 2". Explain it to a third party and confirm nothing feels off
- **Forcing a stop at 5**: 5 is a guideline. Sometimes you reach the root cause in 3, sometimes you need 7. The end point is where "digging further would not change the countermeasure"

**Tips**:
- When a branch appears, track each branch independently (expand into Logic Tree form)
- For each "why" answer, ask yourself "Is that really so? Is there data?"
- Take the root cause to the level of "mechanism, process, structure". Do not attribute it to an individual's ability or motivation
- Countermeasures should address the root cause directly. Distinguish surface-level symptomatic fixes from structural ones

**Next steps**:
- When there are multiple root causes → organize them systematically with the **Cause-and-Effect Diagram**
- Prioritize countermeasures → use the **Urgency/Importance Matrix** or the **Decision Matrix**
- Execution plan for countermeasures → make it concrete with the `/execution` skill
- Build a mechanism to prevent recurrence → use **PDCA** or **KPT** in the `/improvement` skill

---

## 04. Cause-and-Effect Diagram (Fishbone Diagram)
**Purpose**: Identify the causes of a problem systematically

**Template**:
```
            Cause category A ──┐
            Cause category B ──┤
Problem ◀━━━━━━━━━━━━━━━━━━━━━━┤
            Cause category C ──┤
            Cause category D ──┘
```
Typical categories (4M+2 for manufacturing): Man, Method, Material, Machine, Measurement, Environment
Typical categories (4P for services): Policy, Procedure, People, Plant

**How to use**: Place the effect (problem) at the far right, then break down causes in the order of large bones → medium bones → small bones. After brainstorming them, verify with data to identify the true causes.

**Example** (cause analysis of declining customer satisfaction):
```
        Man ──────────────────────────────────────┐
        ├ Share of new hires rose to 40%           │
        ├ Experienced staff keep leaving           │
        └ Training period cut from 2 weeks to 1    │
                                                   │
        Method ───────────────────────────────────┤
        ├ Manual not updated for 3 years           │
        ├ Escalation criteria are vague            │
        └ Customer feedback is shared irregularly  │
                                                   │
Customer satisfaction down 15 pt year over year ◀━━┤
                                                   │
        Machine ──────────────────────────────────┤
        ├ CRM response is slow                     │
        ├ Chatbot answer accuracy is low           │
        └ Phone system wait times are long         │
                                                   │
        Environment ──────────────────────────────┘
        ├ Remote work makes OJT difficult
        ├ Inquiry volume up 150% due to seasonal factors
        └ Competitors' quality improvements raised expectations
```

**Common mistakes**:
- **Wrong category choice**: Applying manufacturing's 4M directly to a service business. Choose categories that fit the industry
- **Stopping at the large bones**: Do not end at "a people problem". Make the medium and small bones concrete. Break down to the level where concrete actions are visible
- **Fixing causes without verification**: The causes you list are only "hypotheses". Back them up with data or on-site confirmation

**Tips**:
- Building it on a whiteboard with the stakeholders gathered brings in multiple perspectives
- Adding "impact: high/medium/low" and "confidence: high/medium/low" to each cause makes priorities clear
- Also pay attention to relationships between causes (example: "people problems" and "method problems" are linked)
- After completion, narrow down to the 3 highest-impact causes and consider countermeasures

**Next steps**:
- Dig into the identified true causes → reach the root with **Why-Why Analysis**
- Structure the causes → organize them MECE with the **Logic Tree**
- Consider countermeasures → use **Brainstorming** or **SCAMPER** in the `/idea` skill
- Manage improvement activities → use **PDCA** in the `/improvement` skill

---

## 05. Logic Tree
**Purpose**: Break a problem or issue down MECE and structure it

**Template**:
```
Theme
├── Major category A
│   ├── Subcategory A-1
│   └── Subcategory A-2
├── Major category B
│   ├── Subcategory B-1
│   └── Subcategory B-2
└── Major category C
    ├── Subcategory C-1
    └── Subcategory C-2
```

**Types**: 
- **What tree (element breakdown)**: Break the whole into its components (example: sales = number of customers x average spend)
- **Why tree (cause investigation)**: Identify the causes of a problem exhaustively
- **How tree (problem solving)**: Break solutions down into concrete actions

**Example** (monthly revenue breakdown of a SaaS service - What tree):
```
Monthly revenue (MRR): 50 million yen
├── New MRR: 8 million yen
│   ├── Via inbound: 5 million yen
│   │   ├── SEO/content: 2 million yen
│   │   ├── Web ads: 2 million yen
│   │   └── Social media/referrals: 1 million yen
│   └── Via outbound: 3 million yen
│       ├── Cold calling: 1 million yen
│       ├── Trade shows/seminars: 1.5 million yen
│       └── Partner referrals: 0.5 million yen
├── Expansion MRR: 4 million yen
│   ├── Upsell: 2.5 million yen
│   └── Cross-sell: 1.5 million yen
├── Retained MRR: 42 million yen
└── Churn MRR: -4 million yen (cancellations)
    ├── Voluntary churn: -3 million yen
    │   ├── Switched to competitors: -1.2 million yen
    │   ├── Budget cuts: -1 million yen
    │   └── Insufficient usage: -0.8 million yen
    └── Involuntary churn: -1 million yen
        └── Payment failure/bankruptcy: -1 million yen
```

**Common mistakes**:
- **Non-MECE breakdown**: Check each level for "gaps" and "overlaps". If unsure, use a known framework (3C, 4P, etc.) as the lens
- **Uneven depth**: Digging deep on one branch while others stay shallow lacks balance. Expand the whole tree evenly to 2 or 3 levels first, then dig into the important branches
- **Stopping after the breakdown**: The tree is a thinking tool. After breaking it down, judge "which branch has leverage" and connect it to action

**Tips**:
- The lens of the first level matters most. If it is wrong, the whole tree is off
- A What tree with numbers is extremely effective for finding bottlenecks (you can see at a glance which branch has the biggest impact)
- A Why tree is Why-Why Analysis expanded sideways. It suits parallel exploration of multiple causes
- Use a How tree to consider actions. Break down until the lowest level is "an action you can execute tomorrow"

**Next steps**:
- Verify each branch → set hypotheses and verification methods with the **Issue Tree**
- Identify bottlenecks → quantify the gap between current and ideal with As-is/To-be
- Evaluate solutions → compare with the **Decision Matrix**
- Elevate to strategy → formulate the overall direction with the `/strategy` skill

---

## 06. MECE
**Purpose**: A thinking frame for identifying elements with no gaps and no overlaps

**Checklist**:
- [ ] Have you defined the whole set?
- [ ] Are there no overlaps between elements? (Mutually Exclusive)
- [ ] Does it cover the whole? (Collectively Exhaustive)
- [ ] Is the lens appropriate? (opposing axes, process, components, etc.)
- [ ] Does the lens fit the purpose? (the best lens differs depending on the purpose of the analysis)

**Typical lenses**: Time series, process order, opposing concepts, existing frames such as 3C/4P, geographic divisions, customer segments

**Example** (analysis of sluggish sales at a restaurant chain - considering lenses for a MECE breakdown):

**Lens 1: Time of day** (MECE)
| Morning (6-11) | Lunch (11-14) | Afternoon (14-17) | Evening (17-22) |
|---|---|---|---|
| Sales share: 5% | Sales share: 40% | Sales share: 15% | Sales share: 40% |
| → Unused | → Stable | → Low utilization | → Declining |

**Lens 2: Customer type** (MECE)
| New customers | Repeaters (1-3 times a month) | Heavy users (weekly or more) |
|---|---|---|
| 30% | 45% | 25% |
| → Flat | → Slight decline | → Sharp decline |

**Lens 3: Revenue structure** (MECE)
- Sales = number of customers x average spend
- Number of customers = seats x turnover rate x business days
- Average spend = food price + drink price + side menu

**Common mistakes**:
- **Falling into perfectionism**: In practice, "roughly MECE" is enough. Do not waste time chasing strict rigor
- **Applying multiple lenses at once**: Mixing several lenses at the same time (example: listing "young people", "Tokyo" and "repeaters" side by side). Apply one lens per level
- **Overusing "Other"**: If the "Other" category accounts for 30% or more of the whole, revisit the lens itself

**Tips**:
- MECE is a "form" and the foundation of all other frameworks. The Logic Tree, Cause-and-Effect Diagram and Issue Tree all assume MECE
- Existing frameworks (3C, 4P, Value Chain Analysis, etc.) are "ready-made products" whose MECE-ness is already verified. Consider applying them before inventing your own lens
- The habit of continually asking "Is this really everything?" matters. Having team members check is also effective
- Choose the lens according to the purpose of the analysis. Even for the same theme, a different purpose calls for a different lens

**Next steps**:
- Practice MECE breakdown → structure with the **Logic Tree**
- Use existing frameworks → use **3C Analysis** or **4P Analysis** in the `/market` skill, or **SWOT Analysis** in the `/strategy` skill
- Dig into customer segments → use the `/customer` skill

---

## 07. Urgency/Importance Matrix
**Purpose**: Organize the priority of tasks and issues in four quadrants

**Template**:
|  | Importance: high | Importance: low |
|---|---------|---------|
| **Urgency: high** | Quadrant 1: Do now | Quadrant 3: Delegate or streamline |
| **Urgency: low** | Quadrant 2: Work on it systematically | Quadrant 4: Reduce or eliminate |

**How to use**: Whether you spend time on Quadrant 2 (important but not urgent) is the key to productivity. If you are always chased by Quadrant 1, a shortage of Quadrant 2 work is often the cause.

**Example** (a startup CTO's quarterly task review):

| | Importance: high | Importance: low |
|---|---------|---------|
| **Urgency: high** | **Do now**: Production server outage response / Applying security vulnerability patches / Handling a bug report from a major customer / Hiring interviews (candidate's deadline at another company is near) | **Delegate or streamline**: Minor bug fixes in internal tools / Writing minutes for regular meetings / Expense reports / First-line inquiry handling |
| **Urgency: low** | **Work on it systematically**: Paying down technical debt / Improving the CI/CD pipeline / 1-on-1s and development of team members / Building a security audit structure / Mid- to long-term architecture design | **Reduce or eliminate**: Weekly reports continued out of inertia / External study groups with little value in attending / Excessive internal chat responses / Unnecessary approval flows |

**Common mistakes**:
- **Everything becomes "urgent and important"**: Make the criteria clear. Judge urgency by "Will a concrete loss occur if we do not act this week?" Judge importance by "Does it directly contribute to reaching the goal six months from now?"
- **Keeping Quadrant 2 on the back burner**: Block concrete time slots on the calendar for Quadrant 2 tasks. Aim to spend 20% or more of the week on Quadrant 2
- **Classifying once and never updating**: Situations change. Review weekly or every two weeks

**Tips**:
- Limit the tasks in each quadrant to about 5 to 7. If there are too many, split them further and make a separate matrix
- When doing this as a team, agree on the definitions of "importance" and "urgency" beforehand
- Have the courage to decide "not to do" Quadrant 4 tasks. Shift the time saved to Quadrant 2
- Quadrant 3 is "tasks you do not have to do yourself". Decide concretely where to delegate (members, outsourcing, tool automation)

**Next steps**:
- Root causes of Quadrant 1 issues → identify structural problems with **Why-Why Analysis** (a shortage of Quadrant 2 work may be the cause)
- Planning for Quadrant 2 → create an execution plan with the `/execution` skill
- Designing delegation to the team → use **RACI** in the `/organization` skill
- Business improvement → use the **Business Flow Diagram** in the `/improvement` skill

---

## 08. Decision Matrix
**Purpose**: Evaluate multiple options quantitatively and choose the best one

**Template**:
| Criterion | Weight | Option A | Option B | Option C |
|---------|-----|--------|--------|--------|
| Criterion 1 | x_ | Score | Score | Score |
| Criterion 2 | x_ | Score | Score | Score |
| Criterion 3 | x_ | Score | Score | Score |
| **Weighted total** | | **_ pts** | **_ pts** | **_ pts** |

**How to use**: Decide the criteria and weights first, then score each option. This structures intuitive judgments. Setting the criteria and weights before looking at the options prevents confirmation bias.

**Example** (selecting a project management tool):
| Criterion | Weight | Jira | Asana | Linear |
|---------|------|------|-------|--------|
| Fit with the development team | x5 | 5 (=25) | 3 (=15) | 5 (=25) |
| Customizability | x4 | 5 (=20) | 3 (=12) | 4 (=16) |
| Low learning cost | x3 | 2 (=6) | 4 (=12) | 4 (=12) |
| Integration with other tools | x3 | 5 (=15) | 4 (=12) | 3 (=9) |
| Cost (annual) | x3 | 3 (=9) | 4 (=12) | 4 (=12) |
| UI/UX comfort | x2 | 2 (=4) | 4 (=8) | 5 (=10) |
| Support quality | x1 | 4 (=4) | 3 (=3) | 3 (=3) |
| **Weighted total** | | **83 pts** | **74 pts** | **87 pts** |

→ In the quantitative evaluation, Linear has the highest score. However, it falls well behind Jira on "integration with other tools", so verify consistency with the existing tool environment before making the final decision.

**Common mistakes**:
- **Setting criteria with the conclusion in mind**: Unconsciously manipulating criteria or weights so that a particular option wins. Set the criteria before examining the options in detail
- **Too many criteria**: Limit to 7 or fewer. With too many, each criterion's weight is diluted and everything converges to the same score
- **Blind faith in the numbers**: The matrix is "a basis for discussion", not "the final conclusion". When scores are close, add qualitative judgment

**Tips**:
- A 5-point scale (1 to 5) is easiest to handle for scoring. A 10-point scale makes the criteria vague
- Set weights from 1 to 5 and aim for a total of around 20, which keeps the criteria balanced
- Have several people score, and discuss the criteria where scores differ widely to surface gaps in understanding
- Apply "fatal criteria" (example: does not meet security requirements) first as cutoff conditions rather than scoring them

**Next steps**:
- Identify options → list them MECE with the **Logic Tree (How tree)**
- Validate the criteria → interview stakeholders → use the `/communication` skill
- Execution plan after selection → make it concrete with the `/execution` skill
- Generate option ideas → use **Brainstorming** in the `/idea` skill

---

## 09. Issue Tree
**Purpose**: Break the question to be solved (the issue) down into verifiable sub-issues

**Template**:
```
Main issue: ________________?
├── Sub-issue 1: ____________?
│   ├── Hypothesis:
│   ├── Verification method:
│   └── Data needed:
├── Sub-issue 2: ____________?
│   ├── Hypothesis:
│   ├── Verification method:
│   └── Data needed:
└── Sub-issue 3: ____________?
    ├── Hypothesis:
    ├── Verification method:
    └── Data needed:
```

**How to use**: Unlike the Logic Tree, each node takes the form of a "question". It is effective when running analysis in a hypothesis-driven way. It is used often in the initial design of consulting projects.

**Example** (considering a growth strategy for a D2C brand):
```
Main issue: Can our D2C brand reach 1 billion yen in sales in 3 years?
│
├── Sub-issue 1: Does a large enough market exist?
│   ├── Hypothesis: The target market is about 50 billion yen a year and growing 8% annually
│   ├── Verification method: Industry report analysis, competitor sales estimates, TAM/SAM/SOM calculation
│   └── Data needed: Yano Research Institute reports, IR materials of listed competitors, Google Trends
│
├── Sub-issue 2: Is there a sustainable differentiator against competitors?
│   ├── Hypothesis: A proprietary raw material sourcing route and customer data use through D2C are the differentiators
│   ├── Verification method: Competitor product comparison, customer interviews (n=30), blind tests
│   └── Data needed: Competitor product samples, existing customer NPS, ingredient analysis results
│
├── Sub-issue 3: Is it profitable at the required customer acquisition cost (CAC)?
│   ├── Hypothesis: If CAC is kept at 8,000 yen or less, an LTV/CAC ratio of 3x or more can be maintained
│   ├── Verification method: Test marketing (3 months), cohort analysis, building an LTV model
│   └── Data needed: Ad operation results, repeat rate trends, churn rate, average spend trends
│
└── Sub-issue 4: Can we secure the resources (people and funds) needed for execution?
    ├── Hypothesis: Hiring 2 additional marketing staff and raising 150 million yen in working capital are needed
    ├── Verification method: Organizational planning, fundraising scenario analysis, VC interviews
    └── Data needed: Hiring difficulty in the talent market, fundraising cases of similar companies, our own BS/PL forecast
```

**Common mistakes**:
- **Not phrased as a question**: Use a question answerable with Yes/No or quantitatively, such as "Does a large enough market exist?" instead of "market analysis"
- **Sub-issues are not MECE**: Check that the sub-issues cover the main issue. Ask yourself "If every sub-issue is answered Yes, can the main issue also be answered Yes?"
- **Unverifiable hypotheses**: Make them verifiable, such as "rated higher than existing products in a blind test" instead of "our product is superior"

**Tips**:
- Setting the main issue matters most. Pose the "right question" and half the analysis is done
- A hypothesis "may be wrong". Having one sets the direction of verification and makes information gathering efficient
- Assigning an "owner" and a "deadline" to each sub-issue makes it work as a project management tool too
- If verification results differ from the hypothesis, update the Issue Tree itself. Treat it as a living document

**Next steps**:
- Verify market-related sub-issues → use **PEST Analysis** and **Five Forces Analysis** in the `/market` skill
- Formulate strategy → use **SWOT Analysis** or the **Ansoff Growth Matrix** in the `/strategy` skill
- Verify customer-related sub-issues → use the **Customer Journey Map** in the `/customer` skill
- Execution plan → set the verification schedule and milestones with the `/execution` skill

---

## How to run the dialogue

### Step 1: Understand the situation

To grasp the user's situation accurately, use AskUserQuestion from the following angles.

**Example questions for the first interview**:

- "What problem or issue are you currently facing? Please be as specific as possible (example: declining sales, worsening operational efficiency, unclear direction for a new business, etc.)"
- "When did the problem start? Was there a triggering event?"
- "What is the purpose of working on this problem? (example: reporting at a management meeting, team improvement activities, personal work improvement, etc.)"
- "Do you have any hypotheses at this point about the causes or solutions?"
- "How much time can you spend on this analysis? (example: I want an overview right now, I want to analyze carefully over a week)"

### Step 2: Propose a framework

Based on the interview, propose 1 or 2 best-fitting frameworks. Explain the reason for the choice clearly.

**Guidelines for proposals**:

| User's situation | Recommended framework | Reason |
|---|---|---|
| "I don't know what the problem is" | As-is/To-be → Logic Tree | First visualize the gap between ideal and current, then break it down structurally |
| "I know the problem but not the cause" | Why-Why Analysis or Cause-and-Effect Diagram | 5 Whys for a single cause, fishbone when multiple causes are suspected |
| "I know the cause but don't know where to start" | Urgency/Importance Matrix | Clarify priorities |
| "There are several solutions and I can't choose" | Decision Matrix | Quantitative comparative evaluation |
| "I want to organize the overall picture of a plan" | 6W2H | Define it exhaustively through 8 lenses |
| "I have a hypothesis but don't know how to verify it" | Issue Tree | Hypothesis-driven analysis design |
| "I'm worried about gaps in the analysis" | MECE → Logic Tree | Ensure completeness of thinking |

### Step 3: Build the worksheet interactively

Present the template and fill it in item by item through dialogue with the user.

**Example questions during the dialogue**:

- "Do you have specific figures or data for this item?"
- "You mentioned 'declining sales'. Specifically, over what period and by what percentage?"
- "Are there other possible factors behind this cause?"
- "How do your team members or manager perceive this problem?"
- "Have you tackled a similar problem before? How did you handle it then?"
- "Who will you report the results of this analysis to, and in what form?"

### Step 4: Complete and output the worksheet

Organize the completed worksheet in Markdown format and output it. Include the following:
- Assumptions and scope of the analysis
- Results of the framework
- 3 to 5 key findings
- Remaining issues and points that need further research

### Step 5: Propose next steps

Based on the analysis results, propose the actions to take next.

**Angles for proposals**:
- Whether to dig deeper with another framework in the same problem skill
- Whether to move to strategy formulation with the `/strategy` skill
- Whether external environment analysis is needed with the `/market` skill
- Whether to deepen customer understanding with the `/customer` skill
- Whether to turn it into an execution plan with the `/execution` skill
- Whether to run an improvement cycle with the `/improvement` skill
- Whether idea generation is needed with the `/idea` skill
- Whether to consider organizational design with the `/organization` skill
- Whether to consider how to communicate to stakeholders with the `/communication` skill
