# Workflow Artifacts

Standard file locations for the spec-copilot workflow.

| Artifact | File | Created By | Used By |
|----------|------|------------|---------|
| **Strategy** | `.spec/strategy.md` | Architect | Planner, Verifier |
| **Plan** | `.spec/plan.md` | Planner | Dispatcher, Verifier |
| **Verification Report** | `.spec/verification.md` | Verifier | Dispatcher, Architect |

## Directory

All artifacts live in `.spec/` at the project root.

```
.spec/
├── strategy.md      # Strategic decisions and rationale
├── plan.md          # Task breakdown with dependencies
└── verification.md  # Gap report from verification
```

## Usage

Agents should:
1. **Read** artifacts from these exact paths
2. **Write** their output to the designated file
3. **Reference** this file when unsure about locations
