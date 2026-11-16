---
source: https://developers.google.com/tech-writing/error-messages/invalid-inputs.md.txt
---

# Identify the user&#39;s invalid inputs

<br />

If the error involves values that the user can enter or modify (for example,
text, settings, command-line parameters), then the error message should identify
the offending value(s).

Not recommended

> Funds can only be transferred to an account in the same country.

Recommended

> You can only transfer funds to an account within the same country. Sender
> account's country (UK) does not match the recipient account's country
> (Canada).

---

Not recommended

> Invalid postal code.

Recommended

> The postal code for the US must consist of either five or nine digits. The
> specified postal code (4872953) contained seven digits.

If the invalid input is a very long value that spans many lines, consider doing
one of the following:

- Disclose the bad input progressively; that is, provide one or more clickable
  ellipses to enable users to control how much additional error information they
  want to see.
- Truncate the bad input, keeping only its essential parts.

### Multiple choice exercise

Which of the following error messages is best? The specified bid ($5) is below
the minimum bid ($8). This answer surfaces the invalid input and provides enough
information for the bidder to compare their bid with the minimum bid. The
specified bid is too low. This error message doesn't surface the invalid input.
The specified bid ($5) is too low. Although this error message does surface the
invalid input, the error message doesn't provide enough information for the user
to fix the problem. The specified bid is below the minimum bid ($8). This answer
doesn't surface the invalid input.

<br />

<br />

**Next unit:**
[Specify requirements and constraints](./technical-writing-error-messages-05-specify-requirements.md)
