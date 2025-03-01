---
id: Accessibility fundamentals
section: accessibility
redirectFrom: /developer-resources/accessibility-guide
---

When it comes to accessibility, there’s always room to improve. That’s why this guide is a work in progress. Your feedback can make it better, so tell us what you think.  

Contribute to our [accessibility documentation](https://github.com/patternfly/patternfly-org) or [reach out to us](https://www.patternfly.org/v4/community/)—we’d love to hear from you!

_“The power of the Web is in its universality. Access by everyone regardless of disability is an essential aspect.”_ — Tim Berners-Lee, W3C Director and inventor of the World Wide Web

When it comes to product experiences, no one should get left behind. That's why accessibility is so important in design and development. The goal of software accessibility is to remove barriers and create inclusive product experiences that work for everyone, regardless of ability.

Accessibility is best achieved when considered early in the design and development process. So if you contribute to PatternFly or use it for your products, familiarize yourself with accessibility first.

## Understanding users’ needs

Great user experiences don’t just happen. They’re designed, tested, and refined with the user in mind. To develop inclusive products, it’s important to understand the varying needs of a wide range of users and consider the assistive tools and methods they use.

This section provides information to help you better understand and address the needs of these [different user groups](https://a11yproject.com/posts/accessibility-is-blind-people/).

**Note**: Some users might fall into multiple groups, and some might use tools created for a different group.
<br />

### Motor

Users with poor motor control can use a range of devices to access contents.

- Users who rely on a keyboard need elements that are keyboard accessible and highly visible when in focus.
- Users who rely on a mouse or touch need target areas that are large enough to be hit easily.
<br />

### No vision

Users with no vision rely on screen readers to access web sites and applications. Often, screen reader users will navigate a page by browsing specific elements, like headers, links, or form elements.

- **Tip:** Use semantic elements and check that labels are meaningful when pulled out of context.

### Low vision

Users with low vision can have different needs depending on the nature of their visual impairment. Users may have difficulty with color differentiation, blurriness, or lack of vision in central or peripheral areas.

- **Tip:** These needs mean that interfaces should not rely on color alone to communicate information, palettes need to have sufficient contrast, and layouts should be responsive when font sizes are increased.
<br />

### Cognitive

Users who have difficulty processing information benefit from well-written content.

- Information should be clear, concise, and easy to scan.
- Consider visual hierarchy, chunk content into short, related sections, and avoid long paragraphs.
<br />
<br />

These are some of the main user groups, but it is not an exhaustive list. Often the “Persona Spectrum”, coined by Microsoft, can be used to understand related mismatches and motivations across a spectrum of permanent, temporary, and situational scenarios.

While accessibility tends to focus on those with disabilities, everyone benefits from accessible products. For example:

- Accessible written content is easier to comprehend for people who aren’t fluent in the language and for people with low literacy levels.
- Alternative text (alt text) makes images accessible to users with low bandwidth connections or with older technologies that can’t load the images.
- Closed captioning benefits those in crowded areas, those teaching children how to read, or those learning a new language.

There are plenty more examples we could include. Essentially, accessibility takes _all users_ into account.

<p className="ws-p pf-v5-u-screen-reader">
  The image below shows that accessibility is a spectrum. Different kinds of cognitive and physical impairments impact how users interact with products. It is important to take all these differing disabilities into account when building accessible products.
</p>

<img src="./PF-a11y.png" alt="Accessibility spectrum image" />
<br />
<br />

## Experience parity

The PatternFly community believes all abilities should be treated equally. In other words, there should be parity in the experience of all users—one user group shouldn't be prioritized over the other.

To help you achieve this, consider these guidelines:

- There should be parity among all input types: touch, mouse, and keyboard.
  - Don’t optimize the experience for one input type at the expense of another.
  - Contents that a user can interact with using a mouse should also be accessible using touch or keyboard.
  - Don’t show interactive elements on hover. Interactive elements that can display in a pop-up must display on click/touch/Enter events.
- There should be parity between the screen reader contents and visibly rendered contents (refer to the [first Note for aria-hidden](https://www.w3.org/TR/wai-aria/#aria-hidden).
- There should be parity between hover and focus events. Any information that’s available on hover for the mouse user should be available on focus for the keyboard-only user. It should also be available to the screen reader user using aria-describedby (refer to [Tooltips & Toggletips example from Inclusive Components](https://inclusive-components.design/tooltips-toggletips/)).

When building accessible user experiences, solving for one can extend to many. Humans are diverse and unique, and inclusive design takes that into consideration to create truly incredible products.  
