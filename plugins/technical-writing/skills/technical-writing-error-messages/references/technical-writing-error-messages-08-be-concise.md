---
source: https://developers.google.com/tech-writing/error-messages/be-concise.md.txt
---

# Be concise

<br />

Write concise error messages. Emphasize what's important. Cut unnecessary text.
See the
[Short sentences unit of Tech Writing One](./technical-writing-one-06-short-sentences.md)
for tips on reducing sentence length.

Not recommended

> Unable to establish connection to the SQL database. _\[Explanation of how to
> fix the issue.\]_

Recommended

> Can't connect to the SQL database. _\[Explanation of how to fix the issue.\]_

---

Not recommended

> The resource was not found and cannot be differentiated. What you selected
> doesn't exist in the cluster. _\[Explanation of how to find valid resources in
> the cluster.\]_

Recommended

> Resource \<name\> isn't in cluster \<name\>. _\[Explanation of how to find
> valid resources in the cluster.\]_

---

Converting from
[passive voice to active voice](./technical-writing-one-04-active-voice.md)
often makes sentences conciser and easier to understand:

Not recommended

> The Froobus operation is no longer supported by the Frambus app.

Recommended

> The Frambus app no longer supports the Froobus operation.

In your enthusiasm to be concise, don't remove so many words that the resulting
error message becomes cryptic. For example, don't reduce the preceding error
message down to the following:

Not recommended

> Unsupported.

### Multiple choice exercise

Reorder and shorten the following start of an error message. How many words can
you remove?

- The SiteID \<SiteID\> you have entered is invalid. 5 Yes. The error should
  read: Invalid SiteID \<SiteID\>. 4 That's a concise error message, but you can
  shorten the error message even more. 3 You can remove more words. None. This
  message is not concise. You can definitely remove some words.

<br />

<br />

**Next unit:**
[Avoid double negatives](./technical-writing-error-messages-09-avoid-double-negatives.md)
