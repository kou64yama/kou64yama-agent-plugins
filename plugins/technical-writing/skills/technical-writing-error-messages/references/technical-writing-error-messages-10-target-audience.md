---
source: https://developers.google.com/tech-writing/error-messages/target-audience.md.txt
---

# Write for the target audience

<br />

Tailor the error message to the target audience. That is:

- Use appropriate terminology for that target audience.
- Be mindful of what the target audience knows and doesn't know.

Beware of the
[curse of knowledge](./technical-writing-one-09-audience.md#curse_of_knowledge)
when writing error messages. A term familiar to you might not be familiar to
your target audience. For example, the following error message contains
terminology appropriate for a target audience of ML experts. If the target
audience includes a significant number of people who aren't ML experts, then the
error message is mystifying:

Recommended for ML experts only

> Exploding gradient problem. To fix this problem, consider gradient clipping.

Now compare the following two error messages. The first error message contains
technical truth, but terms like _server_ , _client_ , _farm_ , and _CPU_ are not
going to help most consumers:

Inappropriate for shoppers

> A server dropped your client's request because the server farm is running at
> 92% CPU capacity. Retry in five minutes.

The second error message is more suitable (and comforting) for a non-technical
audience:

Appropriate for shoppers

> So many people are shopping right now that our system can't complete your
> purchase. Don't worry--we won't lose your shopping cart. Please retry your
> purchase in five minutes.

### Multiple choice exercise

Which audience(s) is the following error message appropriate for?

- This app does not support JPG files. You may only upload SVG or PNG files.
  Software Engineers, System Administrators, and technical end-users All three
  of those audiences understand different file formats. People using an app to
  upload receipts. This error message will frustrate users unfamiliar with file
  formats (which is a lot of people). To become more useful, this error message
  would require additional information explaining how end-users can determine
  file format. Furthermore, some end users don't know what _upload_ means.
  Inappropriate for any audience. Most technical people are familiar with
  different file formats, so this is a good, concise error message for certain
  people.

<br />

<br />

**Next unit:**
[Use terminology consistently](./technical-writing-error-messages-11-use-terminology-consistently.md)
