---
source: https://developers.google.com/tech-writing/accessibility/self-study/sufficient-contrast.md.txt
---

# Use sufficient contrast

<br />

Higher contrast makes it easier for everyone to read text and images. When there
is low contrast, everyone has difficulty viewing content.

Color blindness affects over 300 million people worldwide: 1 in 12 men and 1 in
200 women.

Higher contrast helps people with color blindness and low vision, or anyone that
views a screen in bright sunlight.

Visit
[Colour Blind Awareness](https://www.colourblindawareness.org/colour-blindness/types-of-colour-blindness/)
to learn more about the effects of color blindness.

[WCAG](https://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-contrast.html)
suggests these minimum contrast ratios:

- 4.5:1 for small text
- 3:1 for large text (at least 14 pt bold/18 pt regular)

Consider the following contrast examples:

- Poor contrast

- Better contrast

- Best contrast

## Exercise: Choose colors with sufficient contrast

Complete the following exercise to practice measuring sufficient color contrast:

1. In a separate browser window, open the
   [Contrast Checker](http://webaim.org/resources/contrastchecker) by Web
   Accessibility In Mind (WebAIM).
2. In the contrast checker, enter the following Hex colors to find out which
   foreground-background ratios meet contrast requirements. Record the contrast
   ratios on a notepad or separate document to compare your answers with the
   [possible answers](./technical-writing-accessibility-self-study-04-sufficient-contrast.md#answers).

![](https://developers.google.com/static/tech-writing/images/contrast-exercise.png)

1. First rectangle:
   - Foreground: #148695
   - Background: #FD9C32
2. Second rectangle:
   - Foreground: #EBFF33
   - Background: #667E8B
3. Third rectangle:
   - Foreground: #128697
   - Background: #EAEAEA

**Click the icon to see the expected answers.**

1. First rectangle: FAIL
   - Foreground: #148695
   - Background: #FD9C32
2. Second rectangle: FAIL
   - Foreground: #EBFF33
   - Background: #667E8B
3. Third rectangle: FAIL
   - Foreground: #128697
   - Background: #EAEAEA

Even though some of the pairs may _look_ higher contrast, none of them actually
meets WCAG standards. Unfortunately, "eyeballing it isn't enough"---it's best to
use a contrast checker.

<br />

Use minimum contrast guidelines to ensure that everyone can see your content.

<br />

**Next unit:**
[Choose inclusive language](./technical-writing-accessibility-self-study-05-inclusive-language.md)
