---
name: technical-writing
description:
  Route technical writing requests to the relevant specialist skill. Use for
  documentation, editing, accessibility, and user-facing error messages when the
  appropriate writing focus is not already clear.
---

# Technical Writing Conductor

Choose a specialist based on the user's requested outcome. Read its `SKILL.md`
and follow that guidance to complete the task. If the user names a specialist
directly, choose it.

## Routing

- General technical documentation, explanations, sentences, paragraphs,
  terminology, Markdown, or introductory writing guidance:
  `technical-writing-fundamentals` (default).
- Editing or improving a long document, planning document structure, diagrams,
  code samples, or using LLMs in a writing workflow:
  `technical-writing-advanced`.
- Alt text, inclusive design or language, contrast, visual cues, or an
  accessibility review: `technical-writing-accessibility`.
- Designing, reviewing, or rewriting user-facing error messages:
  `technical-writing-error-messages`.

When a request spans multiple areas, load the smallest set of relevant
specialist skills. For ordinary writing tasks, load fundamentals and add a
specialist only when its focus materially affects the result. Preserve the
user's intended meaning, audience, language, and requested format.

## Specialist skills

- [Fundamentals](../technical-writing-fundamentals/SKILL.md)
- [Advanced](../technical-writing-advanced/SKILL.md)
- [Accessibility](../technical-writing-accessibility/SKILL.md)
- [Error messages](../technical-writing-error-messages/SKILL.md)
