---
name: technical-writing-error-messages
description:
  Design, review, or rewrite user-facing error messages that explain problems
  clearly and help people recover.
---

# Helpful Error Messages

Write an error message as part of a recovery flow. Make the next useful action
clear while protecting diagnostic and sensitive information.

## Workflow

1. Determine who sees the message, where it appears, and what action failed.
   Separate user-facing guidance from logs or developer diagnostics.
2. State what happened in specific, plain language. Name the invalid value or
   field when safe and useful. Explain the cause only when it is known; do not
   guess.
3. Give a concrete recovery action. State relevant requirements and, when it
   clarifies the expected format, show a valid example. Make the action possible
   from the current context when feasible.
4. Be concise, direct, and calm. Avoid blame, jokes that obscure meaning, double
   negatives, unexplained codes, and inconsistent names for the same concept.
5. Match detail to the audience and format the message for scanning. Keep it
   near the problem, ensure dynamically displayed errors are announced to
   assistive technologies, and link to further help when needed.
6. Check edge cases: unavailable services, permission failures, malformed or
   empty input, and cases where the system cannot safely disclose details. Never
   expose secrets, personal data, stack traces, or internal identifiers in
   user-facing copy.
7. Validate the message with realistic examples and, where possible, users or
   support data. Ensure the suggested fix actually resolves the condition.

## References

- [Course overview](references/technical-writing-error-messages-01.md)
- [Error handling](references/technical-writing-error-messages-02-error-handling.md)
- [Identify the cause](references/technical-writing-error-messages-03-identify-the-cause.md)
- [Invalid inputs](references/technical-writing-error-messages-04-invalid-inputs.md)
- [Specify requirements](references/technical-writing-error-messages-05-specify-requirements.md)
- [Show the fix](references/technical-writing-error-messages-06-show-fix.md)
- [Provide examples](references/technical-writing-error-messages-07-provide-examples.md)
- [Be concise](references/technical-writing-error-messages-08-be-concise.md)
- [Avoid double negatives](references/technical-writing-error-messages-09-avoid-double-negatives.md)
- [Target audience](references/technical-writing-error-messages-10-target-audience.md)
- [Consistent terminology](references/technical-writing-error-messages-11-use-terminology-consistently.md)
- [Readable formatting](references/technical-writing-error-messages-12-format-for-readability.md)
- [Tone](references/technical-writing-error-messages-13-set-tone.md)
- [Exercise](references/technical-writing-error-messages-14-want-to-play-a-game.md)
- [Summary](references/technical-writing-error-messages-15-summary.md)
- [Back-end considerations](references/technical-writing-error-messages-16-back-end.md)

Source:
[Writing Helpful Error Messages](https://developers.google.com/tech-writing/error-messages).
