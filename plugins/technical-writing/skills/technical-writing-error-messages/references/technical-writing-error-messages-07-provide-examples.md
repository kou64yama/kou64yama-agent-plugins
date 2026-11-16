---
source: https://developers.google.com/tech-writing/error-messages/provide-examples.md.txt
---

# Provide examples

<br />

Supplement explanations with examples that illustrate how to correct the
problem.

Not recommended

> Invalid email address.

Recommended

> The specified email address (robin) is missing an @ sign and a domain name.
> For example: robin@example.com.

---

Not recommended

> Invalid input.

Recommended

> Enter the pathname of a Windows executable file. An executable file ordinarily
> ends with the .exe suffix. For example: C:\\Program Files\\Custom
> Utilities\\StringFinder.exe

---

Not recommended

> Do not declare types in the initialization list.

Recommended

> Do not declare types in the initialization list. Use calls instead, such as
> 'BankAccount(owner, IdNum, openDate)' rather than 'BankAccount(string owner,
> string IdNum, Date openDate)'

---

Not recommended

> Syntax error on token "\|\|", "if" expected.

Recommended

> Syntax error in the "if" condition. The condition is missing an outer pair of
> parentheses. Add a pair of bounding opening and closing parentheses to the
> condition. For example: if (a \> 10) \|\| (b == 0) # Incorrect if ((a \> 10)
> \|\| (b == 0)) # Correct

### Multiple choice exercise

Which of the following error messages is best for an audience of people who
drive cars?

The specified license plate (QB2 481) is invalid. Valid license plates start
with three uppercase letters and end with three digits. For example: MBR 918 and
NRS 727 are both valid license plates. This error message provides two good
examples of valid license plates. The specified license plate (QB2 481) is
invalid because license plates must start with three letters and end with three
digits. Although this error message surfaces the invalid input and provides an
explanation of what went wrong, this error message lacks an example. The
specified license plate (QB2 481) is invalid. For example: MBR 918 and NRS 727
are both valid license plates. The error message doesn't provide enough context
to make the examples useful. The user might be asking, "Why are MBR 918 and NRS
727 valid but QB2 481 is invalid?"

<br />

<br />

**Next unit:** [Be concise](./technical-writing-error-messages-08-be-concise.md)
