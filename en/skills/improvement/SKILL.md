---
description: "Use the process improvement and optimization frameworks (8 types) interactively"
---

# Process improvement and optimization frameworks

Based on the user's $ARGUMENTS, apply the appropriate framework from the list below.

---

## 01. PDCA
**Purpose**: Improve continuously by running a Plan, Do, Check, Act cycle

**When to use**: When you have a clear goal and want to improve it iteratively. Especially effective for topics where progress can be measured with quantitative indicators.

**Template**:
| Phase | Content | Details |
|---------|------|------|
| **Plan** | Set the goal and the plan | Goal: / Measures: / Schedule: / Success indicators (KPI): |
| **Do** | Execute the plan | What was done: / Records: / Unexpected events: |
| **Check** | Measure and evaluate the results | Goal vs. actual: / Causes of the gap: / Data evidence: |
| **Act** | Feed improvements into the next Plan | Keep doing: / Improve: / Stop doing: / Hypothesis for the next cycle: |

**How to use**: Decide the length of one cycle before you start (weekly, monthly, quarterly, etc.). Do not skip Check.

### Worked example (improving a sales team's close rate)

| Phase | Content | Details |
|---------|------|------|
| **Plan** | Raise the close rate from 20% to 30% | Goal: 30% close rate (in 3 months) / Measures: Introduce a pre-meeting discovery sheet so the customer's problems are understood before every meeting / Schedule: Month 1 = design and test the sheet, Month 2 = everyone uses it, Month 3 = measure the effect / KPI: 100% discovery sheet completion rate, 30% close rate |
| **Do** | Use the discovery sheet in every sales meeting | What was done: Distributed the sheet to all 15 sales reps and ran training. Used in 42 meetings / Records: Completion rate stayed at 85% / Unexpected: Many veteran reps said it was "a hassle" and some sheets were filled in only as a formality |
| **Check** | Close rate 25% (goal missed, but improved) | Goal vs. actual: 25% against a 30% goal (+5 pt improvement) / Causes of the gap: Meetings that used the sheet closed at 33%, but meetings that did not stayed at 18%. Low usage is the bottleneck / Data: 14 of 42 meetings with the sheet closed, 3 of 18 without it closed |
| **Act** | Next cycle focuses on raising the usage rate | Keep: The discovery sheet itself works, keep it / Improve: Cut the sheet's fields from 10 to 5. Build it into the SFA to lower input effort / Stop: Paper-based operation / Hypothesis for the next cycle: If input effort is halved, usage will reach 95% or more and the close rate will hit 30% |

### Common mistakes
1. **Spending too long on Plan**: Chasing a perfect plan and never executing. Start small and get the cycle turning
2. **Skipping Check**: Dropping the evaluation "because we are busy" turns PDCA into mere repetition. Always collect quantitative data
3. **Act becomes a pep talk**: "Try harder" is not an improvement. Write concretely what will change, at the level of actions

### Tips
- Keep each cycle short (about 2 weeks is recommended at first). A long cycle puts Check too far away
- At the Plan stage, define what will count as Check (the judgment of success or failure)
- Record every cycle in a PDCA notebook or spreadsheet so you can track changes between cycles
- The standard approach is to run small PDCA cycles first, then scale up to larger ones

### Next steps
- Want to refine the goal setting → `/execution` (OKR, SMART goals, etc.)
- Want to dig into the root cause of a problem → `/problem` (Why-Why Analysis, Cause-and-Effect Diagram, etc.)
- Want to clarify the division of roles across the team → combine with **06. RACI** in this skill

---

## 02. KPT
**Purpose**: Structure a retrospective into Keep, Problem, and Try

**When to use**: At the end of a sprint, after a project finishes, or for retrospectives in regular meetings. Best for a team session of 30 to 60 minutes.

**Template**:
| Category | Content |
|------|-----|
| **Keep** (things to continue) | - |
| **Problem** (problems and issues) | - |
| **Try** (things to try next) | - |

**How to use**: Start by writing out Keep (positives first). Make the conversion from Problem to Try concrete. Best for a team's regular retrospective.

### Worked example (retrospective of a 2-week sprint)

| Category | Content |
|------|-----|
| **Keep** | - Finishing the daily standup within 15 minutes has become routine. It helps catch blockers early |
|  | - Introducing pair programming cut code review rework by 30% |
|  | - The weekly sync with the designer works, and spec mismatches have disappeared |
| **Problem** | - Tasks piled up in the second half of the sprint, and 3 PRs were merged at the same time on the last day |
|  | - Deploying to the test environment is manual and takes 30 minutes every time |
|  | - Estimates were too optimistic. Only 6 of the 8 planned stories were completed |
| **Try** | - Check the burndown chart mid-sprint (Wednesday) and adjust scope on Thursday if behind |
|  | - Build a CI/CD pipeline for the test environment (Tanaka will start on it next sprint) |
|  | - Apply a buffer factor of 1.3 when estimating. Verify the factor after 3 sprints |

### Common mistakes
1. **No Keeps come out**: A team that only looks at problems burns out. Always start with Keep and list at least 3. Include "things we do well as a matter of course" in Keep
2. **Problems and Tries do not match one-to-one**: Check that every Problem has a Try. A problem without a Try is simply left unattended
3. **Tries are abstract**: Not "improve communication" but "hold a 30-minute sharing session every Friday at 3 pm". State who, when, and what

### Tips
- Use sticky notes (physical or digital). Have everyone write at the same time before sharing, so the loudest voice does not dominate
- Check the status of last time's Tries first. Do not leave them hanging
- When there are too many Problems, vote to prioritize and think of Tries only for the top 3
- Rotate the facilitator every time so every team member owns the retrospective

### Next steps
- Want to dig into individual learning → compare with **03. YWT** in this skill and choose
- Want to analyze the causes of problems structurally → `/problem` (Logic Tree, Why-Why Analysis)
- Want to run improvements continuously → build them into the Do of **01. PDCA** in this skill
- Want to visualize the state of the team → `/organization` (team management frameworks)

---

## 03. YWT
**Purpose**: A retrospective method that extracts learning from "what we did" and connects it to the next action

**When to use**: Personal daily or weekly reports, reflection after training, organizing learning after trying something new. Unlike KPT, it focuses on "learning" rather than "problems", so it suits positive retrospectives.

**Template**:
| Category | Content |
|------|-----|
| **Y** (what we did) | - |
| **W** (what we learned) | - |
| **T** (what to do next) | - |

**How to use**: The difference from KPT is the focus on "what we learned" instead of "problems". Also suits a personal reflection journal.

### Worked example (after customer interviews for a new business)

| Category | Content |
|------|-----|
| **Y** (what we did) | - Ran online interviews with 5 mid-sized companies in the target industry (manufacturing), 60 minutes each |
|  | - Prepared a hypothesis sheet in advance (3 problem hypotheses) and used it as the interview guide |
|  | - Structured the notes the same day after each interview and shared them with the team |
| **W** (what we learned) | - Hypothesis 1, "inventory management is the biggest problem", held for only 1 of 5 companies. The real common problem was "slow information sharing between departments" |
|  | - Decision makers (department head level) and frontline staff see the problems very differently. You cannot see the real picture without interviewing both |
|  | - 60 minutes is not enough for depth. A two-session format, 45 minutes for an overview and a second 30 minutes for depth, gives better quality |
| **T** (what to do next) | - Pivot the hypothesis to "slow information sharing" and map out the specific situations where the problem occurs |
|  | - For the next 5 companies, request interviews with a pair: one decision maker and one frontline person |
|  | - Switch interviews to the two-session format and revise the first-session guide by next Monday |

### Common mistakes
1. **Y becomes a list of activities**: Not just "attended the meeting" but "proposed X at the meeting". Write your own proactive actions
2. **W repeats Y**: "Did interviews, learned interviews are important" contains no learning. Write "what differed from expectations" and "why it happened"
3. **T is too big**: Break it down into actions you can concretely start in the next 1 to 2 weeks

### Tips
- Write it daily as a daily report, and a week's worth compiled becomes a high-quality weekly report
- For W, be aware of both "learning from success" and "learning from failure"
- Reviewing 3 months of YWT reveals your growth patterns and recurring issues
- When used as a team, simply sharing each member's W is a form of knowledge management

### Next steps
- Want to switch to a team retrospective → use **02. KPT** in this skill
- Want to organize learning systematically → `/idea` (mind-map style organization)
- Want to manage the next actions as goals → `/execution` (OKR, task management)

---

## 04. Business Flow Diagram
**Purpose**: Draw the flow of a business process to visualize bottlenecks and waste

**When to use**: Handing over work, the early stage of process improvement, or organizing work that crosses departments. Used to compare the "current state (As-is)" with the "ideal state (To-be)".

**Template**:
```
[Start] → (Decision?) ─Yes→ [Process A] → [Process B] → [End]
                  │
                  No
                  ↓
              [Process C] → [Process B] → [End]
```

**Symbols**:
- `[ ]` = process or task
- `( )` = decision or branch
- `→` = flow
- `[Start/End]` = terminal
- `// //` = waiting time or queue (bottleneck candidate)
- `《 》` = system or tool

**How to use**: First draw the current (As-is) flow, then draw the ideal (To-be) flow and compare them.

### Worked example (improving the expense reimbursement process)

**As-is (current flow)**:
```
[Requester: sorts paper receipts]
    ↓
[Requester: enters amounts in Excel] ← //takes 2 days on average//
    ↓
[Requester: sends to manager by email]
    ↓
//Waiting for manager review: 3 days on average//
    ↓
(Manager: content OK?) ─No→ [Manager: returns by email] → [Requester: corrects] → (loop)
    │
    Yes
    ↓
[Manager: stamps approval and forwards to Accounting]
    ↓
//Waiting for Accounting: 5 days on average//
    ↓
[Accounting: enters manually into the system]
    ↓
[Accounting: processes the bank transfer]
    ↓
[End] ※15 business days on average from request to transfer
```

**To-be (improved flow)**:
```
[Requester: photographs receipt and enters amount in 《Expense app》]
    ↓
[《System》: reads via OCR and checks the amount automatically]
    ↓
[《System》: sends push notification to manager]
    ↓
(Manager: approve in 《App》?) ─No→ [Return with comment in 《App》] → [Requester: corrects] → (loop)
    │
    Yes
    ↓
[《System》: syncs automatically with the accounting system]
    ↓
[Accounting: processes the bank transfer]
    ↓
[End] ※3 business days on average from request to transfer
```

**Improvement effect**: 15 business days → 3 business days (80% shorter). Two manual entry steps automated, waiting time cut with notifications.

### Common mistakes
1. **Starting from the ideal without drawing the current flow**: You cannot improve without an accurate grasp of the current state. Always start from As-is
2. **Inconsistent granularity**: "Prepare the documents" and "stamp the seal" at the same level makes analysis hard. Keep the granularity consistent
3. **Ignoring exception flows**: It is easy to stop at the happy path. The return, error, and exception flows hold the most improvement hints

### Tips
- Note the "time required", "owner", and "tool used" next to each process to sharpen the analysis
- Highlight waiting time (queue time). In most cases waiting time is longer than working time
- Draw it together with the people doing the work. A flow drawn at a desk always differs from reality
- Build the rough flow with sticky notes first, then make a clean copy later

### Next steps
- Want to find the root cause of a bottleneck in the flow → `/problem` (Why-Why Analysis, Cause-and-Effect Diagram)
- Want to eliminate wasteful steps systematically → **07. Muri/Muda/Mura** or **08. ECRS** in this skill
- Want to schedule the improvement project → **05. PERT Chart** in this skill
- Want to communicate the improvement effect to stakeholders → `/communication` (presentation frameworks)

---

## 05. PERT Chart
**Purpose**: Identify the critical path (longest path) from task dependencies and durations

**When to use**: Drafting a project plan, estimating deadlines, optimizing resource allocation. Especially effective for projects where many tasks run in parallel and in series.

**Template**:
| Task | Predecessor | Optimistic (a) | Most likely (m) | Pessimistic (b) | Expected |
|-------|----------|----------|----------|----------|-------|
| A | - | | | | (a+4m+b)/6 |
| B | A | | | | |
| C | A | | | | |
| D | B, C | | | | |

**Critical path**: The path that takes the longest = 

**How to use**: If a task on the critical path slips, the whole project slips. Concentrate resources there.

### Worked example (internal system replacement project)

| Task | Content | Predecessor | Optimistic (a) | Most likely (m) | Pessimistic (b) | Expected (days) |
|-------|------|----------|----------|----------|----------|----------|
| A | Requirements definition | - | 10 | 14 | 21 | 14.5 |
| B | UI/UX design | A | 7 | 10 | 15 | 10.3 |
| C | DB design | A | 5 | 7 | 12 | 7.5 |
| D | Frontend development | B | 14 | 21 | 35 | 22.2 |
| E | Backend development | C | 14 | 21 | 28 | 21.0 |
| F | API integration testing | D, E | 5 | 7 | 14 | 8.2 |
| G | Data migration | C | 7 | 10 | 21 | 11.3 |
| H | User acceptance testing | F, G | 7 | 10 | 14 | 10.2 |

**Path analysis**:
- Path 1: A→B→D→F→H = 14.5 + 10.3 + 22.2 + 8.2 + 10.2 = **65.4 days** (critical path)
- Path 2: A→C→E→F→H = 14.5 + 7.5 + 21.0 + 8.2 + 10.2 = 61.4 days
- Path 3: A→C→G→H = 14.5 + 7.5 + 11.3 + 10.2 = 43.5 days

**Critical path**: A→B→D→F→H (65.4 days). UI/UX design and frontend development are the bottleneck.

**Countermeasure**: Assign additional resources to frontend development (D). Prioritize finalizing the design early.

### Common mistakes
1. **Missing dependencies**: Overlooking a hidden dependency such as "Y cannot actually start until X is done" wrecks the plan
2. **Estimating only with optimistic values**: Downplay the pessimistic value and you will almost certainly slip. Estimate the pessimistic value as "the case where one thing goes wrong"
3. **Neglecting everything off the critical path**: Paths close to the critical path (sub-critical paths) also need attention. A small delay can swap which path is critical

### Tips
- The expected value formula (a+4m+b)/6 is a beta distribution approximation that weights the most likely value 4 times. It is more reliable than intuition
- If you also calculate the standard deviation of the whole project, you can make probabilistic estimates such as "90% chance of finishing within X days"
- Instead of giving buffer days to tasks on the critical path, put a project buffer at the very end of the project (the CCPM approach)
- Update the PERT Chart regularly and track changes in the critical path

### Next steps
- Want to clarify who owns each task → **06. RACI** in this skill
- Want to refine the project's goal setting → `/execution` (WBS, Gantt Chart, OKR)
- Want to identify risk factors → `/problem` (risk matrix, etc.)

---

## 06. RACI
**Purpose**: Clarify the division of roles for each task with 4 types of responsibility

**When to use**: Defining roles at project kickoff, cross-functional projects, sorting out work where "nobody knows who does it". Especially effective when accountability is unclear.

**Template**:
| Task | Person A | Person B | Person C | Person D |
|-------|--------|--------|--------|--------|
| Task 1 | R | A | C | I |
| Task 2 | I | R | A | C |
| Task 3 | C | I | R | A |

**Role definitions**:
- **R**esponsible: The person who does the work. Can be more than one
- **A**ccountable: The final decision maker. **Exactly one per task, always**
- **C**onsulted: People whose opinion is sought beforehand (two-way communication)
- **I**nformed: People told of the result afterward (one-way communication)

### Worked example (new product launch project)

| Task | Product Manager | Engineering Lead | Designer | Marketing | Legal | Executives |
|-------|-------------------|-----------------|----------|-------------|------|-------|
| Product specification | A | C | C | C | I | I |
| UI/UX design | C | C | R/A | I | - | - |
| Development and implementation | C | A | C | I | - | - |
| Quality testing | I | R/A | R | I | - | - |
| Legal review | I | I | - | I | R/A | I |
| Pricing | R | I | - | C | C | A |
| Marketing plan | C | I | C | R/A | C | I |
| Launch decision | R | C | - | C | C | A |
| Press release | C | I | - | R/A | C | I |

### Common mistakes
1. **More than one A**: "Everyone is accountable" is the same as "nobody is accountable". Always narrow A to one person per task
2. **Everyone is C**: Too many consulted people slow down decisions. Make only the people who truly need to be consulted beforehand a C
3. **Making the RACI and stopping there**: After creating it, get the whole team to agree and check for mismatched understanding. Agreement on who is A matters most

### Tips
- List the vertical axis (tasks) first, then fill in the horizontal axis (people or roles)
- A row with both R and A blank is a warning sign that the task is floating with no owner
- Check that A is not concentrated too heavily on one person. Concentration causes bottlenecks
- A blank cell explicitly means "not involved". The blank itself is important information
- Review it regularly. Roles can change as the project progresses

### Next steps
- Want to organize task dependencies and the schedule → **05. PERT Chart** in this skill
- Want assignments that account for team skills and motivation → `/organization` (organization management)
- Want to organize how to communicate with stakeholders → `/communication` (stakeholder communication)
- Want to consider strategic resource allocation → `/strategy` (strategy planning frameworks)

---

## 07. Muri/Muda/Mura (the "Dararin" rule)
**Purpose**: Identify inefficiencies in work from 3 viewpoints

**When to use**: At the early stage of process improvement, when you want to list "what is wrong" exhaustively. A method derived from the Toyota Production System (TPS), applicable not only to manufacturing but also to office work and IT work.

**Template**:
| Viewpoint | Definition | Applicable work | Improvement |
|------|------|------------|-------|
| **Muri** (overburden) | Load beyond capacity | | |
| **Muda** (waste) | Work that creates no value | | |
| **Mura** (unevenness) | Variation in quality or volume | | |

**How to use**: First list the work done on the ground, then label each item as Muri, Muda, or Mura.

### Worked example (improving a customer support department)

| Viewpoint | Definition | Applicable work | Impact | Improvement |
|------|------|------------|------|-------|
| **Muri** | Load beyond capacity | - New hires are put on the phones after 3 days of training. The manual is 500 pages and impossible to absorb | 40% new-hire turnover, 15 complaints per month from wrong answers | - Extend training to 2 weeks - Create a short version of the manual limited to the "top 30 FAQs" - Pair with a veteran for the first month |
| **Muri** | Load beyond capacity | - In peak periods (month end, fiscal year end) each person handles 80 cases a day. Normal periods are 40 | Lower response quality, over 40 hours of overtime a month | - Secure temporary staff for peak periods in advance - Expand the FAQ to raise the self-service rate |
| **Muda** | Work that creates no value | - The same customer data is entered by hand into 3 systems | About 60 hours of duplicated work per month | - Build API integration between the systems so one entry updates all of them |
| **Muda** | Work that creates no value | - After each case a paper report is written and the manager stamps it | 5 minutes per report, 200 cases a month = about 17 hours | - Replace with a status update in the ticket system. The manager checks a dashboard |
| **Mura** | Variation in quality | - Answers differ by agent. A is polite but B is businesslike | Customer satisfaction depends on the agent (NPS varies from 30 to 70) | - Prepare answer templates - Run monthly role-play training - Introduce response quality monitoring metrics |
| **Mura** | Variation in volume | - Inquiry volume varies a lot by weekday (Monday is twice Friday) | Long waits on Monday, surplus staff on Friday | - Optimize shifts by weekday - Strengthen chatbot handling on Mondays |

### Common mistakes
1. **Focusing only on Muda**: Muri (overload) leads to lower quality and turnover, and Mura (variation) hurts the customer experience. Look at all 3 viewpoints in balance
2. **Every improvement is "stop doing it"**: Improving Muri means "reduce the load", improving Mura means "standardize". Each needs a different approach
3. **Analyzing at a desk without listening to the frontline**: Only by observing the actual work and interviewing the people doing it can you see the real Muri, Muda, and Mura

### Tips
- Make a work inventory with the "time required", "frequency", and "owner" of each task before analyzing, and the accuracy improves
- Also refer to the 7 types of waste (Toyota style): overproduction, waiting, transport, over-processing, inventory, motion, defects
- Keep in mind the causal chain "Muri creates Mura, and Mura creates Muda"
- Quantify improvement effects in "time", "cost", and "quality" to make prioritizing easier

### Next steps
- Want to concretely eliminate or improve the inefficiencies you found → **08. ECRS** in this skill
- Want to visualize the flow of work and identify improvement points → **04. Business Flow Diagram** in this skill
- Want to dig into root causes → `/problem` (Why-Why Analysis, Cause-and-Effect Diagram)
- Want to prioritize improvements → `/idea` (evaluation frameworks such as the Payoff Matrix)

---

## 08. ECRS
**Purpose**: Examine process improvements through 4 principles (in order of impact)

**When to use**: After the improvement targets have been identified with a Business Flow Diagram or Muri/Muda/Mura analysis, when examining concrete improvements. Working in the order E→C→R→S lets you start from the most effective improvement.

**Template**:
| Principle | Question | Target work | Improvement | Reduction |
|------|-----|---------|-------|---------|
| **E**liminate | Can we stop doing it? | | | |
| **C**ombine | Can we merge it? | | | |
| **R**earrange | Can we change the order or place? | | | |
| **S**implify | Can we make it simpler? | | | |

**How to use**: Examine in the order E→C→R→S. Eliminate has the biggest impact (stopping is the greatest improvement).

### Worked example (improving monthly report preparation)

**Target**: Monthly report preparation in the sales department (current state: 3 business days every month, 5 people)

| Principle | Question | Target work | Improvement | Reduction |
|------|-----|---------|-------|---------|
| **E**liminate | Can we stop doing it? | - Competitor trend summary (turned out nobody reads it) | Discontinue. Those who need it refer directly to the industry news service | 4 hours/month saved |
| **E**liminate | Can we stop doing it? | - Detailed write-ups of individual deals (the same information is in the SFA) | Replace with the SFA's reporting feature. Stop the double work | 8 hours/month saved |
| **C**ombine | Can we merge it? | - The sales results report and the sales forecast report are prepared separately | Merge into one report. Unify the data source too | 6 hours/month saved |
| **C**ombine | Can we merge it? | - Reported in separate meetings by region and by product | Merge into one monthly all-hands meeting and report via a dashboard | 10 hours/month of meeting time saved |
| **R**earrange | Can we change the order? | - Serial work: aggregate data at month end → write the report at the start of the next month | Automate data aggregation and auto-generate a preliminary version at month end. Next month only add commentary | Lead time 2 days→0.5 days |
| **R**earrange | Can we change the owner? | - The manager handles both data aggregation and analysis | Split the work: an assistant aggregates the data, the manager analyzes | Manager's workload cut 50% |
| **S**implify | Can we make it simpler? | - A 30-page PowerPoint report produced every month | Fix the template and auto-update numbers and charts. Only the comment fields are filled in by hand | 12 hours/month saved |
| **S**implify | Can we make it simpler? | - Internal approval flow for reporting (3 stages) | Simplify approval to 1 stage (department head only). Share the content in real time on a dashboard | Approval wait 3 days→1 day |

**Total improvement effect**: About 40 hours of work saved per month, lead time 3 days→0.5 days

### Common mistakes
1. **Starting from Simplify**: "Efficiency" tends to bring automation and simplification to mind, but asking first whether it can be stopped altogether (Eliminate) has a bigger impact
2. **Deciding instantly that "we cannot stop it"**: "We have always done it" and "management looks at it" are often not the real reasons. Ask concretely "who would be troubled if this work disappeared?"
3. **Not estimating the quantitative effect**: Not "it will probably get easier" but the hours or cost saved in numbers, which makes the proposal easier to get past management

### Tips
- List the target work in advance and know the time required, frequency, and owner of each item before starting
- Put the ECRS results in a table and prioritize in order of the size of the reduction
- To find Eliminate candidates, trace "who uses the output of this work?"
- Drawing business flow diagrams before and after the improvement conveys the change visually
- After implementing improvements, always measure the effect and build it into a PDCA cycle

### Next steps
- Want to make an execution plan for the improvements → **05. PERT Chart** or **06. RACI** in this skill
- Want to monitor improvement effects continuously → **01. PDCA** in this skill
- Want to visualize the flow before and after → **04. Business Flow Diagram** in this skill
- Want to present the improvement proposal to management → `/communication` (Pyramid Structure, PREP)
- Want to design work strategically → `/strategy` (business model design)

---

## How to run the conversation

### Step 1: Hear the problem
Confirm the following with the user:
- **What they want to improve**: A specific business process? How the whole team works? How a project is run?
- **Current sense of the problem**: What do they feel is "not working"? Is there a concrete episode?
- **Purpose of the improvement**: Cost reduction? Quality improvement? Speed? Reducing the burden on staff?
- **Scope**: Individual work? A team? Cross-departmental? Company-wide?
- **Constraints**: Are there constraints on budget, headcount, timeline, or systems?

### Step 2: Propose a framework
Propose the best framework for the problem. Use the selection guide below:

| User's problem | Recommended framework | Reason |
|-------------|----------------|------|
| "I want to do a retrospective" "I want to reflect on the last project" | **KPT** or **YWT** | KPT is for teams, YWT is for individuals and focuses on learning |
| "I want to reduce waste in our work" "I want to be more efficient" | **Muri/Muda/Mura** → **ECRS** | First identify the inefficiencies, then examine concrete improvements |
| "I want to organize the flow of work" "I want to find the bottleneck" | **Business Flow Diagram** | Visualization is the first step |
| "I want to schedule a project" | **PERT Chart** | Plan from task dependencies and durations |
| "I want to clarify who does what" | **RACI** | Visualize the division of roles |
| "I want to keep improving continuously" | **PDCA** | Build an improvement cycle |
| "There are several problems. Where should I start?" | **Muri/Muda/Mura** for the overview → **ECRS** for prioritization | Start with an exhaustive inventory |

Frameworks are often combined. Typical combinations:
- **The classic route for process improvement**: Business Flow Diagram (understand the current state) → Muri/Muda/Mura (identify problems) → ECRS (plan improvements) → PDCA (execute and verify)
- **Project kickoff**: RACI (define roles) → PERT Chart (schedule) → PDCA (track progress)
- **Regular retrospectives**: KPT (team retrospective) → PDCA (execute improvements) → KPT (next retrospective)

### Step 3: Fill in the template interactively
- Do not try to fill in everything at once. Proceed section by section
- When the user's answer is vague, show a concrete example and dig deeper
- Ask "Is there anything else?" to check for omissions
- Show the worked examples as a reference, but have the user fill in the template in their own words

### Step 4: Provide analysis and insights
Once the template is filled in, add analysis from the following angles:
- Point out patterns and trends ("These 3 problems seem to share a root cause")
- Suggest priorities ("From the viewpoint of impact and cost, I recommend tackling them in this order")
- Add viewpoints that are easy to miss ("Let's also consider the impact on stakeholders")

### Step 5: Output the completed worksheet
- Format and output it in Markdown
- Attach a list of next action items as needed
- Suggest connections to other frameworks (other skills)
