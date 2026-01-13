---
name: research-capture
description: Save AI research to dated markdown files. Use when researching topics, gathering information, or exploring questions that should be preserved for future reference.
---

# Research Capture

Save research to markdown files so Claude remembers tomorrow.

## Quick Start

```
/research-capture "What is the Bor Core Four framework?"
```

Creates: `research/2026-01-13-bor-core-four-framework.md`

## Workflow

1. Research the topic (web search, reasoning, synthesis)
2. Create dated file in research/ folder
3. Structure with frontmatter + sections
4. Return file path to user

## Output Format

```markdown
---
date: 2026-01-13
topic: Bor Core Four Framework
sources:
  - https://example.com/source1
  - https://example.com/source2
tags: [frameworks, marketing, strategy]
---

# Bor Core Four Framework

## Summary
[2-3 sentence overview]

## Key Points
- Point 1
- Point 2
- Point 3

## Details
[Expanded research content]

## Sources
- [Source Title](url) - key insight from this source
- [Source Title](url) - key insight from this source

## Questions for Follow-up
- What remains unclear?
- What should be researched next?
```

## File Naming

Pattern: `research/YYYY-MM-DD-topic-slug.md`

Examples:
- `research/2026-01-13-bor-core-four-framework.md`
- `research/2026-01-13-facebook-ads-creative-testing.md`
- `research/2026-01-13-claude-code-plugins.md`

## Guidelines

- Always include sources with URLs when available
- Keep summaries concise (2-3 sentences)
- Tag for discoverability
- End with follow-up questions to guide future research
- Create research/ folder if it doesnt exist

## Why This Matters

Tomorrow, when you ask Claude about this topic, itll find this file. The paper trail compounds. Each research session builds on the last instead of starting from scratch.
