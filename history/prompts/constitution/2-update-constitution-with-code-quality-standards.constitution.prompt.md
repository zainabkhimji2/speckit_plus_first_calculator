---
id: 2
title: Update constitution with code quality standards
stage: constitution
date: 2025-11-14
surface: agent
model: gemini-pro
feature: none
branch: {{BRANCH}}
user: SARS
command: update @.specify/memory/constitution.md to improve Code Quality Standards- All functions must include type hints on parameters and return types  - Example: `def add(a: float, b: float) -> float:`- All functions must include docstrings explaining what they do  - Example: `"""Add two numbers and return the sum."""`- Follow PEP 8 naming conventions (lowercase_with_underscores for functions)- Lines must be under 100 characters- No magic numbers; use named constants  - Bad: `if x > 10:`  - Good: `if x > MAX_POWER_EXPONENT:'
labels: ["constitution", "update", "code-quality"]
links:
  spec: null
  ticket: null
  adr: null
  pr: null
files:
  - .specify/memory/constitution.md
tests:

---

## Prompt

update @.specify/memory/constitution.md to improve Code Quality Standards- All functions must include type hints on parameters and return types  - Example: `def add(a: float, b: float) -> float:`- All functions must include docstrings explaining what they do  - Example: `"""Add two numbers and return the sum."""`- Follow PEP 8 naming conventions (lowercase_with_underscores for functions)- Lines must be under 100 characters- No magic numbers; use named constants  - Bad: `if x > 10:`  - Good: `if x > MAX_POWER_EXPONENT:'

## Response snapshot

New version: 0.2.0 (Minor bump for adding code quality standards)
Files flagged for manual follow-up:
*   .specify/templates/plan-template.md
*   .specify/templates/spec-template.md
*   .specify/templates/tasks-template.md
*   .specify/templates/commands/*.md
Suggested commit message: `docs: update constitution to v0.2.0 (add code quality standards)`

## Outcome

- ✅ Impact: Constitution updated with new code quality standards.
- 🧪 Tests: N/A
- 📁 Files: Updated `.specify/memory/constitution.md`
- 🔁 Next prompts: User to review and confirm.
- 🧠 Reflection: Successfully updated the constitution based on user input. Need to ensure dependent templates are updated manually.

## Evaluation notes (flywheel)

- Failure modes observed: None
- Graders run and results (PASS/FAIL): N/A
- Prompt variant (if applicable): N/A
- Next experiment (smallest change to try): N/A
