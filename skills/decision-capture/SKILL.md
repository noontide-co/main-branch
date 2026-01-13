---
name: decision-capture
description: Record business decisions with context and reasoning. Use when making choices, resolving questions, or committing to a direction that should be documented.
---

# Decision Capture

Record decisions so you never relitigate the same question twice.

## Quick Start

```
/decision-capture "We're going with Stripe over Square for payment processing"
```

Creates: `decisions/2026-01-13-stripe-over-square.md`

## Workflow

1. Understand the decision and context
2. Ask clarifying questions if needed (options considered, reasoning)
3. Create dated file in decisions/ folder
4. Structure with frontmatter + ADR format
5. Return file path to user

## Output Format

```markdown
---
date: 2026-01-13
decision: Stripe over Square for payment processing
status: decided
stakeholders: [Devon, Matt]
tags: [payments, infrastructure, tools]
---

# Stripe Over Square for Payment Processing

## Context
[What situation prompted this decision?]

## Decision
[The actual decision in one clear sentence]

## Options Considered
1. **Stripe** - [pros/cons]
2. **Square** - [pros/cons]
3. **Other** - [why ruled out]

## Reasoning
[Why this option won]

## Consequences
- [What this enables]
- [What this prevents]
- [What this costs]

## Review Date
[When to revisit, if applicable]
```

## File Naming

Pattern: `decisions/YYYY-MM-DD-decision-slug.md`

Examples:
- `decisions/2026-01-13-stripe-over-square.md`
- `decisions/2026-01-13-three-tier-pricing.md`
- `decisions/2026-01-13-github-for-premium-access.md`

## Status Values

- `proposed` - Under consideration
- `decided` - Committed, implementing
- `superseded` - Replaced by newer decision
- `deprecated` - No longer relevant

## Guidelines

- One decision per file
- Include options that were rejected (future you will wonder why)
- Tag for discoverability
- Link to related decisions if applicable
- Create decisions/ folder if it doesnt exist

## Why This Matters

Six months from now, youll ask "why did we choose Stripe?" This file answers that question instantly. No archeology through Slack. No relitigating. The decision is documented with full context.
