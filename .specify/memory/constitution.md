<!--
Sync Impact Report:
Version change: 0.1.0 → 0.2.0
List of modified principles:
- [PRINCIPLE_1_NAME] → Test-Driven Development (TDD)
- [PRINCIPLE_2_NAME] → Modern Python & Type Hinting
- [PRINCIPLE_3_NAME] → Clean Code & Readability
- [PRINCIPLE_4_NAME] → Architectural Decision Records (ADRs)
- [PRINCIPLE_5_NAME] → Object-Oriented Principles
Added sections: Technical Stack & Quality Requirements, Code Quality Standards
Removed sections: None (repurposed existing sections)
Templates requiring updates:
- .specify/templates/plan-template.md: ⚠ pending
- .specify/templates/spec-template.md: ⚠ pending
- .specify/templates/tasks-template.md: ⚠ pending
- .specify/templates/commands/*.md: ⚠ pending
Follow-up TODOs: None
-->
# CLI Calculator Project Constitution

## Core Principles

### I. Test-Driven Development (TDD)
All new features and bug fixes MUST be developed using a Test-Driven Development (TDD) approach. Tests MUST be written and approved before implementation begins, following a strict Red-Green-Refactor cycle.

### II. Modern Python & Type Hinting
All Python code MUST use Python 3.12+ and include comprehensive type hints for all functions, methods, and variables to improve code clarity and maintainability.

### III. Clean Code & Readability
Code MUST be clean, self-documenting, and easy to read. Adherence to established style guides and best practices is mandatory.

### IV. Architectural Decision Records (ADRs)
All significant architectural decisions MUST be documented using Architectural Decision Records (ADRs) to capture context, options considered, and rationale.

### V. Object-Oriented Principles
Development MUST adhere to essential Object-Oriented Programming (OOP) principles, including SOLID, DRY (Don't Repeat Yourself), and KISS (Keep It Simple, Stupid).

## Technical Stack & Quality Requirements

### Technical Stack
- **Language:** Python 3.12+
- **Package Manager:** UV
- **Testing Framework:** pytest
- **Version Control:** All project files MUST be managed in Git.

### Quality Requirements
- All tests MUST pass.
- Code coverage MUST be at least 80%.
- Data structures MUST utilize Python dataclasses.

### Code Quality Standards
- All functions MUST include type hints on parameters and return types. Example: `def add(a: float, b: float) -> float:`
- All functions MUST include docstrings explaining what they do. Example: `"""Add two numbers and return the sum."""`
- Follow PEP 8 naming conventions (lowercase_with_underscores for functions).
- Lines MUST be under 100 characters.
- No magic numbers; use named constants. Bad: `if x > 10:` Good: `if x > MAX_POWER_EXPONENT:`

## Governance
This Constitution supersedes all other practices. Amendments require documentation, approval, and a migration plan. All Pull Requests (PRs) and code reviews MUST verify compliance with these principles.

**Version**: 0.2.0 | **Ratified**: 2025-11-14 | **Last Amended**: 2025-11-14