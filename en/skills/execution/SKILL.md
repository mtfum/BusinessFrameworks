---
description: "Apply the goal setting and execution management frameworks (9 types) interactively"
---

# Goal setting and execution management frameworks

Based on the user's $ARGUMENTS, apply the appropriate framework from the list below.

---

## 01. OKR (Objectives and Key Results)
**Purpose**: Link ambitious objectives to quantitative key results and align the direction of the organization

**When to use**: When an organization or team wants to clarify "what we aim for" and get everyone moving in the same direction. Especially effective for companies in a growth phase or when launching a new business.

**Template**:
| Level | Objective | Key Result 1 | Key Result 2 | Key Result 3 |
|-------|-----------------|-------------|-------------|-------------|
| Company | | | | |
| Team | | | | |
| Individual | | | | |

**Rules**:
- Objectives are qualitative and challenging (something that excites people)
- Key Results are quantitative and measurable (60-70% achievement is the ideal difficulty)
- Set and review them every quarter
- 2 to 5 Key Results per Objective is appropriate (too many blurs the focus)
- Do not tie OKRs directly to the performance evaluation system (it discourages taking on challenges)

**Worked example (SaaS company)**:
| Level | Objective | Key Result 1 | Key Result 2 | Key Result 3 |
|-------|-----------------|-------------|-------------|-------------|
| Company | Build a product-led growth engine and become the No. 1 HR tech company in Japan | ARR 500M JPY → 800M JPY | NPS 40 → 60 | Churn rate 3% → 1.5% |
| Team (Product) | Deliver a product experience users want to use every day | DAU/MAU ratio 30% → 50% | Onboarding completion rate 40% → 75% | Feature request response rate 60% → 80% |
| Individual (Engineer) | Achieve both product reliability and development speed | Deploy frequency weekly → daily | Production incidents 3/month → 0/month | PR review wait time 24h → 4h |

**Common mistakes**:
- **Key Results are actually tasks**: "Write 10 blog posts" is a task, not a Key Result. Define Key Results as outcomes, such as "Organic traffic 5,000 → 15,000 per month"
- **The Objective is too bland**: "Increase sales" gives no sense of direction. Use wording that fires up the team, such as "Become the de facto standard in the XX industry"
- **Company OKRs and team OKRs are unrelated**: OKRs at each level must connect logically to the goal above them. Aim for roughly 60% alignment rather than a complete cascade

**Tips**:
- Start with 1 to 3 Objectives for the whole company. Too many OKRs is the same as prioritizing nothing
- Check Key Result progress in a weekly 15-minute check-in. A review only at quarter end is too late
- Separating "Committed OKRs" (must achieve) from "Aspirational OKRs" (stretch) makes them easier to run
- When introducing OKRs, pilot them with one team first, then roll out company-wide

**Next steps**:
- Break Key Results into factors → **02. KPI Tree**
- Turn each Key Result into concrete actions → **03. SMART**
- Evaluate OKR achievement from multiple angles → **07. Balanced Scorecard (BSC)**
- Sort out the strategic direction first → `strategy` skill (SWOT Analysis, Porter's generic strategies)
- Clarify role assignments in the team → `organization` skill (RACI)

---

## 02. KPI Tree
**Purpose**: Break the final goal (KGI) into factors and clarify the KPIs and owners at each layer

**When to use**: When you want to break a large goal such as "increase sales" or "reduce costs" into concrete actions. Especially effective for businesses that can be managed by numbers.

**Template**:
```
KGI: Sales XX JPY
├── KPI: Number of customers × Average spend per customer
│   ├── KPI: Number of new customers
│   │   ├── KPI: Number of leads × CVR
│   │   └── Owner: Marketing
│   └── KPI: Existing customer LTV
│       └── Owner: Customer Success
└── ...
```

**How to use**: Build the tree backward from the KGI. Attach an owner and actions to each KPI. Each breakdown should be either an addition (A = B + C) or a multiplication (A = B × C).

**Worked example (e-commerce site)**:
```
KGI: Monthly sales 50M JPY
├── New customer sales = Number of new buyers × First purchase value
│   ├── Number of new buyers = Site visits × Purchase CVR
│   │   ├── Site visits = 500K/month → Target: 700K/month
│   │   │   ├── Ad traffic: 200K → Target: 300K (Owner: Ad operations team)
│   │   │   ├── SEO traffic: 150K → Target: 200K (Owner: Content team)
│   │   │   └── Social media traffic: 150K → Target: 200K (Owner: Social media team)
│   │   └── Purchase CVR = 2.0% → Target: 2.8% (Owner: UI/UX team)
│   └── First purchase value = 4,500 JPY → Target: 5,000 JPY (Owner: Merchandising)
├── Existing customer sales = Number of repeat buyers × Repeat purchase value × Purchase frequency
│   ├── Number of repeat buyers = Previous month's buyers × Repeat rate
│   │   └── Repeat rate = 25% → Target: 35% (Owner: CRM)
│   ├── Repeat purchase value = 6,000 JPY → Target: 7,000 JPY (Owner: Merchandising)
│   └── Purchase frequency = 1.2 times/month → Target: 1.5 times/month (Owner: CRM)
```

**Common mistakes**:
- **The breakdown logic is broken**: "Sales = Number of customers × Average spend" is correct, but mixing in a metric that cannot be computed directly, such as "brand awareness", breaks the consistency of the tree
- **Too many leaf KPIs to manage**: Breaking down to 4 or more levels leaves the front line unsure of what to track. Limit each team to 2 or 3 KPIs
- **KPIs without actions**: A KPI Tree is a map of "what to measure". It only works when paired with an action plan for "how to improve"

**Tips**:
- First check whether the goal can be broken down with basic arithmetic. If not, consider a method other than the KPI Tree (such as BSC)
- Record the "current value", "target value" and "gap" for each KPI, and improve the KPI with the largest gap first
- Operation sticks when you build a weekly dashboard that tracks KPIs automatically
- A KPI Tree is a "hypothesis". Review its structure periodically

**Next steps**:
- List improvement measures for each KPI → `idea` skill (Brainstorming)
- Dig into the bottleneck KPI → `problem` skill (Logic Tree, Why-Why Analysis)
- Design KPIs for SaaS/apps → **04. AARRR (Pirate Metrics)**
- Revisit the KGI itself → **01. OKR**
- Raise KPIs by improving business processes → `improvement` skill (Value Stream Mapping)

---

## 03. SMART
**Purpose**: Make goals concrete and actionable using five criteria

**When to use**: When you want to turn a "vague" goal into one that is "ready to act on". Effective for personal goal setting, defining project milestones and team action plans.

**Template**:
| Criterion | Check | Content |
|------|---------|------|
| **S**pecific | □ | What will you achieve? |
| **M**easurable | □ | How will you measure it? What are the numbers? |
| **A**chievable | □ | Is it realistically achievable? |
| **R**elevant | □ | Is it aligned with the higher-level goal? |
| **T**ime-bound | □ | By when? |

**SMART goal statement**: "By [deadline], improve the [metric] of [specific target] from [current value] to [target value]."

**Worked example (marketing team)**:

Vague goal: "We want more social media followers"

| Criterion | Check | Content |
|------|---------|------|
| **S**pecific | ✅ | Grow the follower count of the official X account and establish it as a lead generation channel |
| **M**easurable | ✅ | Followers 5,000 → 15,000, leads via X 20/month → 80/month |
| **A**chievable | ✅ | Competitor B achieved growth of the same scale over the same period. Two content team members have already been added |
| **R**elevant | ✅ | Directly tied to the company OKR "Raise the inbound marketing ratio to 50%" |
| **T**ime-bound | ✅ | By the end of September 2026 (6 months) |

**SMART goal statement**: "By the end of September 2026, grow the official X account's followers from 5,000 to 15,000 and raise leads via X from 20 per month to 80 per month."

**Common mistakes**:
- **Underestimating Achievable**: Do not judge by willpower ("we can do it if we try"). Verify feasibility objectively from past data, resources and competitor cases
- **Confusing Measurable with Specific**: Specific defines the scope of "what to do". Measurable defines the metric for "how success is measured". Both are needed
- **Skipping Relevant**: Without checking alignment with the higher-level goal, you end up with "the goal was achieved but it did not contribute to the business"

**Tips**:
- Use SMART as a "goal quality checklist". First write the goal freely, then polish it against the five SMART items
- When used in a team, have members peer review each other's goals in pairs to raise accuracy
- An extended version, "SMARTER", adds Evaluated and Recognized
- Aim for a single goal statement that contains all five elements

**Next steps**:
- Turn the SMART goal into an execution plan → **06. Gantt Chart**
- Line up multiple SMART goals on a timeline → **05. Roadmap**
- Check the strategy above the goal → **01. OKR**
- List obstacles to achieving the goal → `problem` skill (Issue Tree)
- Communicate the goal to stakeholders → `communication` skill (Pyramid Structure)

---

## 04. AARRR (Pirate Metrics)
**Purpose**: Manage service growth through a five-stage funnel

**When to use**: When you want to manage growth systematically for a digital product such as a web service, app or SaaS. Ideal for startup PMF validation and prioritizing growth hacking measures.

**Template**:
| Stage | Definition | Current value | Target value | Key measures |
|------|------|-------|-------|---------|
| **A**cquisition | Users learn about the service | | | |
| **A**ctivation | First value experience | | | |
| **R**etention | Repeated use | | | |
| **R**eferral | Recommending to others | | | |
| **R**evenue | Payment and monetization | | | |

**Golden rule**: Improve Retention first, then invest in Acquisition. Pouring water into a leaky bucket is pointless.

**Worked example (task management SaaS)**:
| Stage | Definition | Metric | Current value | Target value | Key measures |
|------|------|------|-------|-------|---------|
| **A**cquisition | New visits | Monthly unique visitors | 50,000 | 80,000 | Strengthen SEO, comparison article landing pages, Product Hunt listing |
| **A**ctivation | First value experience | 5 or more tasks created within 7 days of sign-up | 25% | 45% | Improve onboarding flow, provide templates, tutorial videos |
| **R**etention | Continued use | Monthly retention rate (M2) | 35% | 55% | Optimize push notifications, encourage team invites, habit-forming nudges |
| **R**eferral | Referrals | Invite feature usage rate | 5% | 15% | Invite incentives, stronger share features, team plan discounts |
| **R**evenue | Payment | Free-to-paid conversion rate | 3% | 7% | Redesign the value gate, promote annual plans, expand enterprise plans |

**Common mistakes**:
- **Overweighting Acquisition**: Chasing only acquisition numbers and continuing to spend on ads while activation and retention are broken. The result is a soaring CAC (customer acquisition cost) and LTV < CAC
- **Vague definition of Activation**: Treating "sign-up" as Activation. Activation should be defined as the point where the user experiences the Aha! moment (the moment they feel the value)
- **Building the funnel once and leaving it**: The metrics at each stage need redefining as the product matures. The metrics to track differ between Series A and Series C

**Tips**:
- Define the Aha! moment for each stage. Example: Activation = "the moment a user invites one team member and they complete a task together"
- Combine with cohort analysis to track improvement trends over time
- Pick just one bottleneck (the stage with the worst numbers) and improve it intensively
- Decide on one North Star Metric and focus on the AARRR stage that affects it most

**Next steps**:
- Break down the KPIs at each stage in detail → **02. KPI Tree**
- Dig into why customers drop off → `customer` skill (Customer Journey Map)
- Analyze competitors' growth strategies → `market` skill (competitor analysis)
- Generate ideas for measures → `idea` skill (Brainstorming, SCAMPER)
- Sort out the product strategy → `strategy` skill (Lean Canvas)

---

## 05. Roadmap
**Purpose**: Visualize medium- to long-term plans on a timeline and manage milestones

**When to use**: When sharing quarterly to yearly plans with stakeholders. Used in product development, business planning and organizational change to agree on "when, what and in which order".

**Template**:
| Period | Q1 | Q2 | Q3 | Q4 |
|------|----|----|----|----|
| Theme | | | | |
| Milestones | | | | |
| Key tasks | | | | |
| Resources | | | | |
| Risks | | | | |

**How to use**: An overly detailed roadmap goes stale. Focus on showing the major milestones and the direction.

**Worked example (B2B SaaS product)**:
| Period | Q1 (Strengthen foundation) | Q2 (Accelerate growth) | Q3 (Expand market) | Q4 (Maximize revenue) |
|------|--------------|--------------|--------------|----------------|
| Theme | PMF validation and foundation | Self-serve growth | Enterprise expansion | Profitability improvement |
| Milestones | Reach NPS 50, complete core features | Exceed MRR 10M JPY | 3 large enterprise customers onboarded | Reach ARR 200M JPY |
| Key tasks | Rebuild API foundation, UX redesign | Revise pricing plans, invite feature | SSO/SAML support, audit logs | Promote annual plans, upsell features |
| Resources | 5 engineers, 1 designer | +2 marketers | +2 enterprise sales reps | +2 CS staff |
| Risks | Development delays from technical debt | Competitor price offensive | Scope creep in enterprise requirements | Worsening churn rate |

**Common mistakes**:
- **Treating the roadmap as a "promise"**: A roadmap is an "agreement on direction", not a promise of a detailed schedule. Build it on the assumption that it will be updated every quarter as conditions change
- **Cramming in everything**: Limit each quarter to 1 or 2 themes. "This and that too" means nothing gets finished
- **Leaving the risk row blank**: Anticipating risks in advance speeds up decisions when the plan changes

**Tips**:
- Create three kinds of roadmap: (1) for executives (yearly, strategic themes), (2) for the team (quarterly, milestones), (3) for customers (next quarter, features)
- A simple "Now / Next / Later" roadmap also works. It shows only priority without fixing dates
- Always define "success criteria (Definition of Done)" for each milestone
- As a guideline, review the roadmap monthly and revise it substantially once a quarter

**Next steps**:
- Break each milestone into detailed tasks → **06. Gantt Chart**
- Make the success criteria for milestones concrete → **03. SMART**
- Sort out the strategic rationale for the roadmap → `strategy` skill (SWOT Analysis, Ansoff Growth Matrix)
- Analyze risks in detail → `problem` skill (Risk Matrix)
- Explain the roadmap to stakeholders → `communication` skill (PREP)

---

## 06. Gantt Chart
**Purpose**: Manage project tasks, owners, durations and dependencies in one view

**When to use**: When you want to manage task order and parallel work in a concrete project (product release, event preparation, system migration, etc.). Ideal for projects of about 2 weeks to 3 months.

**Template**:
| Task | Owner | Start | End | W1 | W2 | W3 | W4 | Depends on |
|-------|------|-------|-------|----|----|----|----|------|
| | | | | ██ | | | | |
| | | | | | ██ | ██ | | Task 1 |
| | | | | | | ██ | ██ | Task 2 |

**How to use**: Manage delay risk with the critical path (the longest path) in mind. If a task on the critical path slips by one day, the whole project slips by one day.

**Worked example (new feature release project)**:
| Task | Owner | Start | End | W1 | W2 | W3 | W4 | W5 | W6 | Depends on |
|-------|------|-------|-------|----|----|----|----|----|----|------|
| Requirements definition | PM Tanaka | 7/1 | 7/11 | ██ | ██ | | | | | - |
| UI design | Designer Suzuki | 7/7 | 7/18 | | ██ | ██ | | | | Requirements definition (50%) |
| API design | Engineer Sato | 7/14 | 7/18 | | | ██ | | | | Requirements definition |
| Frontend implementation | Engineer Yamada | 7/21 | 8/1 | | | | ██ | ██ | | UI design |
| Backend implementation | Engineer Sato | 7/21 | 8/1 | | | | ██ | ██ | | API design |
| Integration testing | QA Takahashi | 8/4 | 8/8 | | | | | | ██ | FE implementation, BE implementation |
| Release preparation | PM Tanaka | 8/4 | 8/8 | | | | | | ██ | Integration testing (parallel) |
| **Critical path**: Requirements definition → UI design → FE implementation → Integration testing (30 business days total) |

**Common mistakes**:
- **No buffer**: If every task is scheduled at its shortest estimate, one delay topples the rest like dominoes. Reserve a buffer of 10 to 20% of the total on the critical path
- **Vague dependencies**: Instead of "just run things in parallel somehow", define explicitly that "Task B cannot start until Task A is complete"
- **Neglecting updates**: A Gantt chart is a living thing. Reflect actuals at least once a week and reschedule immediately when there is a delay

**Tips**:
- Tasks are easiest to manage at a granularity "one person can complete in 1 to 5 days"
- There are four kinds of dependency: FS (finish-to-start), SS (start-to-start), FF (finish-to-finish), SF (start-to-finish). FS is the most common
- Place milestones (zero-duration events) at key points as progress checkpoints
- When there is a lot of parallel work, watch for resource conflicts (multiple tasks piling up on the same person)

**Next steps**:
- Check where the project sits in the bigger picture → **05. Roadmap**
- Decide task priorities → `idea` skill (Payoff Matrix)
- Analyze problems blocking project progress → `problem` skill (Why-Why Analysis)
- Sort out role assignments in the team → `organization` skill (RACI)
- Cut waste in the process → `improvement` skill (Value Stream Mapping)

---

## 07. Balanced Scorecard (BSC)
**Purpose**: Evaluate and manage the business in a balanced way from four perspectives, not just finance

**When to use**: When financial metrics alone do not show the whole picture of the business. Effective for mid-term business planning, cross-departmental goal setting and executive dashboard design. Works especially well on balance problems such as "sales are up but the organization is exhausted".

**Template**:
| Perspective | Strategic objective | KPI | Target value | Action |
|------|---------|-----|-------|----------|
| **Financial** | | | | |
| **Customer** | | | | |
| **Internal process** | | | | |
| **Learning and growth** | | | | |

**Cause and effect**: Learning and growth → Internal process improvement → Higher customer satisfaction → Financial results
(Causality chains from bottom to top. Tell a story in which every perspective ultimately leads to financial results.)

**Worked example (mid-sized manufacturer)**:
| Perspective | Strategic objective | KPI | Current value | Target value | Action |
|------|---------|-----|-------|-------|----------|
| **Financial** | Improve profitability | Operating margin | 5% | 8% | Increase the share of high value-added products |
| **Financial** | Grow new businesses | Share of sales from new businesses | 5% | 15% | Invest 100M JPY in each of 3 new businesses |
| **Customer** | Improve customer loyalty | NPS | 30 | 50 | Build a customer success organization |
| **Customer** | Solution proposal capability | Share of proposal-led deals | 20% | 40% | Shift to consultative sales |
| **Internal process** | Shorten development lead time | Planning to mass production period | 18 months | 12 months | Introduce an agile development process |
| **Internal process** | Improve quality | Defect rate | 0.5% | 0.1% | Introduce an AI inspection system |
| **Learning and growth** | Develop digital talent | Number of DX training graduates | 50 people | 200 people | Company-wide DX training program |
| **Learning and growth** | Raise engagement | Employee engagement score | 3.2 | 4.0 | Introduce 1-on-1s, clarify career paths |

**Cause-and-effect story**: Develop DX talent (learning and growth) → Make the development process more efficient (internal process) → Strengthen solution proposal capability (customer) → Improve profitability (financial)

**Common mistakes**:
- **The four perspectives are independent**: The KPIs in each perspective are scattered with no cause-and-effect story. Make clear "why this learning leads to this process improvement"
- **Leaning toward the financial perspective**: The essence of BSC is managing "leading indicators other than finance". Ten financial KPIs and one of each other kind is meaningless
- **Neglecting learning and growth**: It is easy to put in formal KPIs such as "number of training sessions". Set metrics that measure "whether skills actually improved and were applied to work"

**Tips**:
- Use BSC together with a "strategy map", a diagram that visualizes the cause-and-effect relationships between the four perspectives with arrows
- Limit KPIs to 2 to 4 per perspective. 12 to 16 in total is the upper limit
- Distinguish "lagging indicators (results)" from "leading indicators (drivers)". Example: sales (lagging) ← number of sales meetings (leading)
- Review the scorecard every quarter and verify whether the cause-and-effect hypotheses were correct

**Next steps**:
- Break down the financial perspective KPIs in detail → **02. KPI Tree**
- Make the strategic objectives in each perspective concrete → **03. SMART**
- Dig into the internal process perspective → `improvement` skill (Value Stream Mapping, Six Sigma)
- Design organizational measures for learning and growth → `organization` skill (McKinsey 7S)
- Sort out the direction of company strategy → `strategy` skill (SWOT Analysis, Porter's generic strategies)

---

## 08. OODA Loop
**Purpose**: A thinking cycle for deciding and acting fast in a rapidly changing environment

**When to use**: Situations that demand speed, such as emergencies with no time to plan, responding to competitor moves, sudden market shifts and hypothesis testing for new businesses. Where PDCA cycles in the order "plan, do, check", OODA goes "observe, judge, act immediately" and is far faster.

**Template**:
| Phase | Question | Content |
|---------|------|------|
| **O**bserve | What is happening? | Collect raw data without bias |
| **O**rient | What does it mean? | Interpret it with experience, knowledge and context |
| **D**ecide | What will we do? | Choose a course of action from several options |
| **A**ct | Move now | Execute and feed the results back into the next Observe |

**Difference from PDCA**:
| | PDCA | OODA |
|--|------|------|
| Starting point | Plan | Observe |
| Speed | Medium to slow (time spent on planning) | Fast (from observation straight to action) |
| Suited to | Stable environments, quality control | Uncertain environments, competitive situations |
| Cycle | Weeks to months | Hours to days |

**Worked example (responding to a competitor's price offensive)**:
| Phase | Question | Content |
|---------|------|------|
| **O**bserve | What is happening? | Competitor A cut the price of its flagship product by 30%. It went viral on social media, and inquiries to us dropped 40% from last week. Three existing customers contacted us saying they are "considering switching". The sales team reports that "deals have stalled" |
| **O**rient | What does it mean? | Competitor A has just raised funding and is in a share-expansion phase. Joining a price war would be a war of attrition. However, if we do not stop short-term customer outflow, churn will spike. Our strengths are "customer support quality" and "the breadth of API integrations" |
| **D**ecide | What will we do? | (1) Existing customers: the CS team immediately offers every customer an individual "loyalty discount (15% off the annual plan)". (2) New prospects: create ROI comparison materials and compete on "total cost of ownership" rather than price. (3) Product: launch a new landing page that promotes the advantage of our API integrations |
| **A**ct | Execute | Distribute the script to the CS team today. Finish the ROI comparison materials this week. Publish the landing page next week. → Observe the results again in one week |

**Common mistakes**:
- **Confusing Observe with Orient**: Observe is "collecting facts". Orient is "interpreting facts". "The competitor cut prices" is Observe. "They are starting a war of attrition" is Orient. Separating them raises the quality of decisions
- **Bias in Orient**: Interpreting data through past successes and assumptions. Consciously ask "is there another interpretation?"
- **Not returning to Observe after Act**: Stopping after one pass is just an ad hoc response. The essence is to observe the results and keep running the loop at high speed

**Tips**:
- OODA's greatest weapon is "the speed and depth of Orient". Building up industry knowledge, customer understanding and competitor intelligence every day sharply raises the accuracy of Orient
- Run each loop within one week at most. "I want more data" is the trap of analysis paralysis
- When used in a team, split the Observe role (information gathering) from the Orient role (analysis) so they can work in parallel
- Use OODA for the most urgent matters and PDCA for themes that deserve careful work

**Next steps**:
- Systematize information gathering for the Observe phase → `market` skill (PEST Analysis, Five Forces Analysis)
- Understand customers deeply to raise the accuracy of Orient → `customer` skill (Persona, Empathy Map)
- Expand the options for Decide → `idea` skill (Brainstorming, SCAMPER)
- Review the results of Act in a structured way → `improvement` skill (PDCA, KPT)
- Explain the decision to stakeholders → `communication` skill (PREP, Pyramid Structure)

---

## 09. Organization Chart
**Purpose**: Visualize the organization's structure, chain of command and areas of responsibility

**When to use**: Organization design, reorganization, launching a new team, post-M&A integration, new employee orientation, etc. When you want to clarify "who is responsible for what and who reports to whom".

**Template**:
```
              [CEO]
        ┌───────┼───────┐
   [Business A] [Business B] [Admin]
      ┌──┴──┐             ┌──┴──┐
    [Dev] [Sales]      [HR] [Finance]
```

**Types of organizational structure and their characteristics**:
| Structure | Characteristics | Advantages | Disadvantages | Suited to |
|------|------|---------|----------|----------|
| Functional | Divided by function such as sales, development and admin | Deeper expertise, economies of scale | Prone to silos | Small and mid-sized single-business companies |
| Divisional | Divided by product, region or customer | Fast business decisions, clear P/L responsibility | Duplicated functions, company-wide optimization is hard | Diversified companies |
| Matrix | Managed on two axes, function × business | Flexible resource allocation | Complex chain of command, conflicts | Global companies |
| Project-based | Teams formed per project | Purpose-specific, speed | Weaker sense of belonging | IT, consulting |

**Worked example (SaaS company with about 50 people)**:
```
                    [CEO / Representative Director]
            ┌───────────┼───────────┐
        [CTO]        [COO]        [CFO]
     Technology     Business    Administration
    ┌───┴───┐    ┌───┴───┐    ┌───┴───┐
[Product] [SRE] [Sales] [CS]  [HR] [Finance]
 Dev team  Infra Sales team CS   HR   Finance
   (15)    (3)     (8)    (6)  (2)    (2)
     │               │       │
  ┌──┴──┐        ┌──┴──┐   │
[FE] [BE] [QA]  [Enterprise] [SMB] [Onboarding]
 (5)  (7)  (3)      (5)      (3)       (3)

Note: The design team (3) reports directly to the CTO and supports every team across the board
Note: Marketing (4) reports directly to the COO and works across Sales and CS
```

**Common mistakes**:
- **Being satisfied with just drawing the chart**: An organization chart is only boxes lined up. It does not work unless the "mission, authority and scope of responsibility" of each box is written down
- **The chart diverges from reality**: The official chart and the actual decision-making flow often differ. Also understand the informal lines of power
- **Choosing a structure that does not fit the size**: A matrix organization is overkill for a 10-person company. The standard approach is to start with a functional organization and consider a divisional structure once you pass 30 people

**Tips**:
- Creating a "responsibility assignment matrix (RACI)" alongside the chart clarifies ambiguous roles
- The ideal "span of control (the number of people one manager can directly manage)" is 5 to 8
- Do not reorganize more than once every six months. Frequent changes confuse the front line
- Deliberately look for "blank zones" in the chart (areas nobody owns). That is where risk hides
- In the remote work era, it also helps to visualize a "communication map (who interacts with whom on a daily basis)" in addition to the official chart

**Next steps**:
- Clarify role assignments for each position → `organization` skill (RACI)
- Diagnose the organization's strengths and weaknesses → `organization` skill (McKinsey 7S)
- Plan an organizational transformation → **05. Roadmap**
- Design team motivation → `organization` skill (Motivation-Hygiene Theory)
- Propose a reorganization to executives → `communication` skill (Pyramid Structure, PREP)

---

## How to run the conversation

### Step 1: Interview
Use AskUserQuestion to confirm the following:

1. **Goal and challenge**: "What do you want to achieve?" "What is your biggest problem right now?"
2. **Time horizon**: "By when do you want to achieve it?" (short term: 1 to 3 months / medium term: 3 to 12 months / long term: 1 year or more)
3. **Scope**: "Which level are we talking about: individual, team, department or company?"
4. **Current state**: "Tell me about the current situation (with specific numbers if you have them)"
5. **Constraints**: "Are there budget, staffing or technical constraints?"

### Step 2: Select a framework
Based on the interview results, propose the most suitable framework. Use the following criteria:

| Need | Recommended framework |
|-------|----------------|
| Align the direction of the whole organization | **01. OKR** |
| Break a numerical goal into factors | **02. KPI Tree** |
| Make a vague goal concrete | **03. SMART** |
| Manage growth metrics for a web service/app | **04. AARRR** |
| Visualize a medium- to long-term plan | **05. Roadmap** |
| Manage project tasks | **06. Gantt Chart** |
| Evaluate the business from multiple angles | **07. BSC** |
| Make decisions fast | **08. OODA Loop** |
| Design/visualize the organizational structure | **09. Organization Chart** |

When several frameworks apply, propose a combination. Example: "Let's first set the direction with OKR, break down the metrics with a KPI Tree, and then build the execution plan with a Gantt Chart."

### Step 3: Fill in the template interactively
- Do not ask everything at once. Proceed section by section through dialogue
- When the user's answer is vague, show concrete examples and offer options
- Customize the worked examples to the user's industry and business model
- Insert interim confirmations along the way, such as "Let me confirm what we have so far"

### Step 4: Complete and review
- Output the completed worksheet in Markdown
- Add comments on "points to improve" and "perspectives that are easy to overlook"
- As "next steps", suggest connections to other frameworks and skills

### Combination patterns for multiple frameworks

**Pattern A: End-to-end from strategy to execution**
`strategy` (SWOT, etc.) → **01. OKR** → **02. KPI Tree** → **06. Gantt Chart**

**Pattern B: Growth hacking**
`customer` (Persona) → **04. AARRR** → **02. KPI Tree** → `idea` (generate measures)

**Pattern C: Mid-term business plan**
**07. BSC** → **01. OKR** → **05. Roadmap** → **09. Organization Chart**

**Pattern D: Crisis response**
**08. OODA Loop** → `problem` (root cause analysis) → **03. SMART** (make countermeasures concrete)
