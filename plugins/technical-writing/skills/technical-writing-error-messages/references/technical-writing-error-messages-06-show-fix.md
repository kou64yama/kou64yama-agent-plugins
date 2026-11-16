---
source: https://developers.google.com/tech-writing/error-messages/show-fix.md.txt
---

# Explain how to fix the problem

<br />

Create **actionable error messages**. That is, after explaining the cause of the
problem, explain how to fix the problem.

Not recommended

> The client app on your device is no longer supported.

Recommended

> The client app on your device is no longer supported. To update the client
> app, click the **Update app** button.

Here's a second example:

Not recommended

> Could not fetch resource:
>
> - Quota 'CPUS' exceeded. Limit: 1.0 in region us-central-1.

Recommended

> You requested 2.0 CPUs, which exceeds your quota of 1.0 CPUs in the
> us-central-1 region. To fix the problem, take either of the following actions:
>
> - Increase your CPU quota in the us-central-1 region.
> - Make your request in a region where you have more CPU quota. See _\[URL of
>   documentation\]_ for details.

<br />

**Next unit:**
[Provide examples](./technical-writing-error-messages-07-provide-examples.md)
