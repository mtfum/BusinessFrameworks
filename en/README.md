# Business Frameworks for Claude Code

A Claude Code plugin for working through business frameworks interactively.
It proposes the framework that best fits your problem, then completes a worksheet with you through dialogue.

English translation of the Japanese plugin in this repository ([README](../README.md)).

## Included frameworks (9 categories, 73 frameworks)

| Category | Skill | Count | Main frameworks |
|---------|---------|:-----:|----------------|
| Problem discovery and definition | `problem` | 9 | As-is/To-be, Why-Why Analysis, Logic Tree, MECE, Issue Tree |
| Macro environment and industry analysis | `market` | 7 | PEST Analysis, Five Forces, 3C Analysis, SWOT, Value Chain |
| Customer understanding and market segmentation | `customer` | 8 | Persona, Empathy Map, Customer Journey, Jobs to Be Done, STP |
| Idea generation and evaluation | `idea` | 9 | Mandalart, SCAMPER, Design Thinking, Osborn's Checklist |
| Strategy and business model design | `strategy` | 10 | BMC, Lean Canvas, Blue Ocean, 4P Analysis, AIDMA |
| Goal setting and execution management | `execution` | 9 | OKR, KPI Tree, SMART, AARRR, Balanced Scorecard |
| Process improvement and optimization | `improvement` | 8 | PDCA, KPT, YWT, RACI, ECRS |
| Organization and team management | `organization` | 9 | MVV, Will/Can/Must, Johari Window, GROW Model |
| Communication and presentation | `communication` | 4 | PREP, TAPS, Pyramid Structure, Elevator Pitch |

## Installation

```bash
/plugin install business-frameworks-en --marketplace mtfum/BusinessFrameworks
```

## Usage

### Start from the main menu

```
/business-frameworks-en:framework
```

Describe your problem and Claude proposes the best-fitting frameworks.

### Pick a category directly

```
/business-frameworks-en:strategy
/business-frameworks-en:problem
/business-frameworks-en:customer
```

### Name a framework

```
/business-frameworks-en:strategy SWOT Analysis
/business-frameworks-en:idea Mandalart
/business-frameworks-en:execution OKR
```

### Test locally

```bash
git clone https://github.com/mtfum/BusinessFrameworks.git
cd BusinessFrameworks
claude --plugin-dir ./en
```

## Directory layout

```
en/
  .claude-plugin/
    plugin.json            # plugin manifest (business-frameworks-en)
  skills/
    framework/SKILL.md     # main entry (full list, automatic proposal)
    problem/SKILL.md       # problem discovery and definition
    market/SKILL.md        # macro environment and industry analysis
    customer/SKILL.md      # customer understanding and market segmentation
    idea/SKILL.md          # idea generation and evaluation
    strategy/SKILL.md      # strategy and business model design
    execution/SKILL.md     # goal setting and execution management
    improvement/SKILL.md   # process improvement and optimization
    organization/SKILL.md  # organization and team management
    communication/SKILL.md # communication and presentation
```

## License

MIT
