# Accessibility on the Web

By transcribing historical documents, edition projects contribute to providing low-barrier access to our historical heritage, which should not be compromised by a non-navigable platform.
In the context of research data, the term "accessibility" is often understood in relation to the FAIR principles, while the abbreviation "a11y" refers specifically to accessibility.

The accessibility of a digital edition starts with the data and extends through the platform's design all the way to its implementation.

## Considerations When Creating Edition Data

- Choice of language(s)
- Alternative text for images
- Semantic versus non-semantic markup (`<strong>` or `<span style="font-weight: bold;">`)
- Using semantic markup instead of plain text (`<app><lem wit="#h">frey</lem><rdg wit="#V">free</rdg></app>` instead of `frey ] h; free V`)
- Structuring the content according to the document (pages and lines) or the content itself (chapters and paragraphs)

## Special Challenges for Texts in Digital Editions

- Index Annotations:

    - Too many links in a text can be distracting. Dropdowns require special attention when checking for accessibility barriers.
    - An alternative or supplement to dropdowns could be a list of relevant entries for each document.

- Footnotes and Comments:

    - Footnotes only make sense in their context. When displayed in a separate list, they should be linked on both ends (as in TEI Publisher).
    - Footnotes in dropdowns retain context but have the same issues as index annotations.
    - Editorial comments with a lemma are also understandable even without the primary text.

- Underlining, Additions, Deletions, Superscripts:

    - Avoiding the interpretation of markup and simply reproducing it visually can make these elements invisible.

- Parallel Texts:

    - Depending on the edition's intent and the length of the parallel texts, tables or chapters are appropriate for displaying them.

- Competing Hierarchies: 
    
    - The presentation in the digital edition versus the structure of the original document.

## Challenges in Navigation in Digital Editions

- Pagination for Longer Documents:

    - Each view should be treated as a separate document and needs a unique title for identification.
    - Switching between views can make navigation unclear and harder to follow.

- Information Density per Screen

## Links

-   [Web Content Accessibility Guidelines (WCAG) 2.1](https://www.w3.org/TR/WCAG21/){:target="\_blank"} with internationally valid recommendations from W3C
-   [eCH-0059 Accessibility Standard](https://www.ech.ch/de/ech/ech-0059/3.0){:target="\_blank"} for public authorities and licensed companies in Switzerland
-   [Accessibility in the CMS of the University of Zurich](https://t.uzh.ch/access){:target="\_blank"} with various links to instructions and tools
-   [Handouts of the Centre for Digital Editions ZDE Zurich](https://www.zde.uzh.ch/de/offers/handout.html)
