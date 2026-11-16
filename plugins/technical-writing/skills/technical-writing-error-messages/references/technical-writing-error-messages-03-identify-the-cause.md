---
source: https://developers.google.com/tech-writing/error-messages/identify-the-cause.md.txt
---

# Identify the error&#39;s cause

<br />

Tell users exactly what went wrong. Be specific---vague error messages frustrate
users.

Not recommended

> Bad directory.

Recommended

> The _\[Name of directory\]_ directory exists but is not writable. To add files
> to this directory, the directory must be writable. _\[Explanation of how to
> make this directory writable.\]_

---

Not recommended

> Invalid field 'picture'.

Recommended

> The 'picture' field can only appear once on the command line; this command
> line contains the 'picture' field _\<N\>_ times. Note: Prior to version 2.1,
> you could specify the 'picture' field more than once, but more recent versions
> no longer support this.

<br />

<br />

**Next unit:**
[Identify the user's invalid inputs](./technical-writing-error-messages-04-invalid-inputs.md)
