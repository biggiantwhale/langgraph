# Fable5-Style Workflow

This document defines a safe, model-agnostic workflow for getting stronger results from ChatGPT, Claude, Gemini, Copilot, Cursor, Codex, or any other AI coding assistant.

This does **not** unlock or emulate a proprietary model. It only applies a stricter reasoning, verification, and review process.

## Purpose

Use this workflow for:

- coding tasks
- AI automation projects
- GitHub portfolio work
- documentation
- debugging
- business automation demos
- external client deliverables

## Core principle

Do not ask the AI to simply produce an answer. Ask it to produce an answer, verify it, find weaknesses, and compress it into an executable next action.

## Standard task prompt

```text
Work in a Fable5-style senior-engineer mode.

Goal:
[write the exact task]

Context:
[files, constraints, target user, platform, deadline]

Rules:
- Be direct and practical.
- Do not invent facts, files, APIs, or dependencies.
- Break the work into small verifiable steps.
- Check for edge cases and risks.
- Give one best option, not many vague options.
- End with the next concrete action.

Output format:
1. Goal
2. Plan
3. Implementation
4. Verification
5. Risks
6. Score
7. Next action
```

## Code review prompt

```text
Review this work in Fable5-style senior-engineer mode.

Check:
- correctness
- bugs
- missing edge cases
- security/safety risk
- maintainability
- performance
- business usefulness
- portfolio value

Return:
1. Score out of 100
2. Critical issues
3. Improvements
4. Final recommended version
5. Next action
```

## Business automation prompt

```text
Assess this idea as an AI automation service.

Judge by:
- can I build it quickly?
- does it solve a real business pain?
- can I charge for it?
- can it become a reusable template?
- can it become portfolio evidence?
- what is the smallest demo version?

Return:
1. Score
2. Target customer
3. Service package
4. Demo structure
5. Price range
6. Outreach message
7. Next action today
```

## Debugging prompt

```text
Debug this step by step.

Rules:
- Do not guess blindly.
- Identify the smallest failing unit.
- Give likely causes ranked by probability.
- Provide one fix at a time.
- Explain how to verify each fix.

Return:
1. Suspected cause
2. Evidence
3. Fix
4. Verification
5. If it still fails, next check
```

## Recommended scoring

Use this scorecard when evaluating work:

| Area | Weight |
|---|---:|
| Correctness | 30 |
| Practical execution | 20 |
| Maintainability | 15 |
| Business value | 15 |
| Portfolio value | 10 |
| Risk control | 10 |

## For this user workflow

The default decision filter is:

```text
Does this make money?
Can it be executed now?
Can it become portfolio evidence?
Can it become a reusable service?
What is the one next action?
```

## Recommended GitHub use

Store results as:

```text
.github/copilot-instructions.md
prompts/
docs/
examples/
portfolio/
```

Recommended first portfolio project:

```text
AI automation portfolio
- Google Sheets sales/customer management sample
- RFQ/quote automation sample
- document summarization workflow
- outreach message templates
- before/after screenshots
```

## Safety note

Avoid unofficial account bypass tools, private backend scraping, shared tokens, and tools that require copying login cookies. Use official products or local prompt/workflow improvements whenever possible.