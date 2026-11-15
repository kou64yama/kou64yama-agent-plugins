---
source: https://developers.google.com/tech-writing/error-messages/use-terminology-consistently.md.txt
---

# Use terminology consistently

<br />

Use terminology consistently for all error messages within a single product
area. If you call something a "datastore" in one error message, then call the
same thing a "datastore" in all the other error messages.

Not recommended

> Can't connect to cluster at 127.0.0.1:56. Check whether minikube is running.

Recommended

> Can't connect to minikube at 127.0.0.1:56. Check whether minikube is running.

> [!NOTE] **Note:** Some authoring systems automatically recommend synonyms to
> ensure that you don't keep repeating the same word. Yes, variety spices up
> paragraphs. However, variety in error messages can confuse users.

Error messages must appear consistently with similar formats and
non-contradictory content; that is, the same problem must generate the same
error message. For example, if different parts of an app each detect problems
with internet connection, both parts should emit the same error message.

<br />

<br />

**Next unit:**
[Format error messages to enhance readability](./technical-writing-error-messages-12-format-for-readability.md)
