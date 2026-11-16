---
source: https://developers.google.com/tech-writing/accessibility/self-study/editing-accessibility.md.txt
---

# Edit for accessibility

<br />

In this unit, you learn how to edit your own and others' writing to make it more
accessible to all users. The unit focuses on ways to write---and edit---your
documentation to make it accessible to everyone. This unit is not meant as an
exhaustive reference, but it does describe some general best practices for
editing documentation to focus on accessibility.

## Cultivate an accessibility mindset for doc editing

When you are aware of and focus on the fundamentals of good writing, you also
make your documentation more accessible.

With practice, self-editing can help you catch accessibility pitfalls, such as
these:

- poor or missing headings
- uninformative link text
- dense, complex text

## Create helpful headings

Headings help your audience understand what's in your document. Clear,
well-structured document headings simplify navigation for people with cognitive
disabilities and those who use screen readers.

- Tag headings with heading elements.
  - HTML: `<h1>`, `<h2>`, `<h3>` ...
  - Markdown: `#`, `##`, `###` ...
- Use a level-1 heading for the page title or main content heading.
- Don't skip levels of the heading hierarchy. For example, don't jump from an
  `<h1>` to an `<h3>`.

References:

- [Headings and titles](https://developers.google.com/style/headings)
- [Cognitive accessibility design pattern: Make the site hierarchy easy to understand and navigate](https://www.w3.org/WAI/WCAG2/supplemental/patterns/o2p02-site-structure/)
- [Making content usable for people with cognitive and learning disabilities](https://www.w3.org/TR/coga-usable/#summary-find)

## Include informative link text

People who use screen readers often use them to scan a page to hear just the
links. Use informative link text to ensure that your audience hears meaningful
information, not just "Learn more, learn more, learn more."

- Avoid:
  - [Learn more](https://developers.google.com/style/tables)
  - [Click here](https://developers.google.com/style/tables)
  - [This document](https://developers.google.com/style/tables)
- Good:
  - Learn how to [format tables](https://developers.google.com/style/tables).
  - Read about
    [machine learning](https://developers.google.com/machine-learning).

> **Bonus:** Informative link text also improves search engine optimization.

Reference: [Link text](https://developers.google.com/style/link-text)

## Use straightforward language and short sentences

Other units in this course talk about making visual images accessible to
everyone. Remember that abstract and unfamiliar _written_ representations can
also be particularly challenging for users with cognitive or visual impairments.

Avoid unfamiliar jargon, US-based slang, pop-cultural references, and
complicated linguistic constructions. Use active voice and short sentences, and
define your technical terms on first use if they are not commonly understood.

References:

- [Active voice](https://developers.google.com/style/voice)
- [Jargon](https://developers.google.com/style/jargon)
- [Designs that make use of abstract imagery and metaphors](https://www.w3.org/TR/coga-usable/#amy-scenario-3-designs-that-make-use-of-abstract-imagery-and-metaphors)

## Exercise: Edit a document

In this exercise, you edit a short document to make it more accessible.

Focus on the order in which the information is presented; place writing tips
first. Simplify the wording where possible. You can change anything, but
especially look for accessibility pitfalls such as missing or unnecessary
headings, uninformative link text, and dense, complex text.

Whenever possible, streamline and simplify the wording. This suggestion isn't
accessibility-specific; however, as with many writing tips, good writing is good
for accessibility.

Now, make a copy of the following exercise and edit it for accessibility.

> ### A list of reasons why simplifying a document through editing is good
>
> Determine whether or not you can simplify your document through the use of
> terminology that is equivalent but relatively shorter in length and therefore
> more easily comprehensible by your audience. It's important to make sure your
> document is edited before it is seen by your audience, which might include
> people that are less or more familiar with the matter covered by your
> document.
>
> Step 1
>
> The first thing you need is a rough draft. Some things that can help make your
> document easier to read are making sure you have links to background
> information, and also checking for active voice instead of passive voice. If
> you have long sentences you can consider shortening them or implementing the
> use of a list to make the information easier to scan.
>
> Step 2
>
> The second thing you need is a list of resources that will help you edit, like
> [this page](https://developers.google.com/style/).
>
> Also
> [this other one is good,too](https://learn.microsoft.com/en-us/style-guide/accessibility/writing-all-abilities).
>
> Once you have editing resources to use as you edit, you can use them to edit
> your document.

### Tips for getting started

The title of the exercise is _A list of reasons why simplifying a document
through editing is good_; one approach might be to look for language that could
be presented in a bulleted list or lists.

Highlight or otherwise identify phrases that could work as bulleted items. Start
to build your bulleted list (or lists). As you do so, look for ways to make
complex text simpler by using active voice and short phrases. Revise link text
to be informative. Keep list items parallel.

#### Build your bulleted list

The following table shows how you might begin to break down the longer
paragraphs into concise bulleted lists.

|---|---|---| | **Existing text** | **Possible list items** | **Edited list
items** | | Paragraph 1: Determine whether or not you can **simplify your
document** through the use of **terminology that is equivalent but relatively
shorter in length** and therefore more easily **comprehensible by your
audience**. | - Determine whether or not you can **simplify your document**. -
Use **terminology that is equivalent but relatively shorter in length.** - Make
sure your material is **comprehensible to your audience**. | - **Simplify**: Use
short sentences. - Check **terminology**: If you use words that might be
unfamiliar to your audience, include definitions. - _Note: The second bullet
covers this already._ | | Paragraph 2: It's important to **make sure your
document is edited** before it is seen by **your audience** , **which might
include people that are less or more familiar**with the matter covered by your
document. | - Make sure your document is **edited**. - _Note: You've already
addressed the need to **know your audience**. You can cut this repetitive
information._ | - **Edit**: Request a review or peer edit from someone who is
familiar with your subject matter. |

> > [!NOTE] **Note:** Learn more about creating lists in
> > [Tech Writing One](../../technical-writing-fundamentals/references/technical-writing-one-07-lists-and-tables.md).

If you continue breaking down the existing text into possible bulleted items,
you can organize and order the items logically, which will make the information
easier for your readers to understand and act on.

#### Click the icon to see a possible answer.

Before you share a document, use these basic editing techniques to make sure
that your audience can understand your message.

- Simplify: Use short sentences.
- Use active voice: Change passive voice to active voice.
- Include lists: If possible, change long paragraphs to lists to make
  information easier to scan.
- Know your audience: Focus on the needs and knowledge level of your potential
  users.
- Check terminology: If you use words that might be unfamiliar to your audience,
  include definitions.
- Provide background information: Include links to resources that your audience
  might find useful.
- Edit: Request a review or peer edit from someone who is familiar with your
  subject matter.

Read more about writing and editing documentation for accessibility in the
following resources:

- [_Google developer documentation style guide_](https://developers.google.com/style)
- [_Microsoft style guide:_ Writing for all abilities](https://learn.microsoft.com/en-us/style-guide/accessibility/writing-all-abilities)

---

## Test your content for accessibility

Finally, to get a feel for some different ways your users might access and
consume your document, try these testing tips:

- Change the zoom level to help accommodate readers on small screens or
  full-size monitors.
- Use only the keyboard to navigate your document. For example, see
  [Keyboard shortcuts in Chrome](https://support.google.com/chrome/answer/157179).
- Use a screen reader:
  - ChromeVox for ChromeOS
  - VoiceOver for Mac

These methods can help you assess the usability of your document for different
audiences as you edit your own and others' documents for accessibility.

<br />

**Next unit:**
[Conclusion](./technical-writing-accessibility-self-study-08-conclusion.md)
