# Accessibility in the Web

With the transcription of historical documents, edition projects contribute to low-barrier access to historical heritage, which must not be lost through a non-navigable platform.
In the field of research data, the English equivalent "accessibility" is often understood in the context of the FAIR principles, while the abbreviation "a11y" refers exclusively to accessibility.

The accessibility of a digital edition begins with the data and extends from the design of the platform to its implementation.

## Considerations when creating the edition data

- Choice of language(s)
- Alternative texts for images
- Semantic or non-semantic markup (`<strong>` or `<span style="font-weight: bold;">`)
- Semantic markup instead of simple text (`<app><lem wit="#h">frey</lem><rdg wit="#V">free</rdg></app>` instead of `frey ] h; free V`)
- Orientation of the structure to the document (pages and lines) or to the content (chapters and paragraphs)

## Special challenges for texts in digital editions

- Index annotations:

    - Many links in a text can be disruptive. Dropdowns deserve special attention when checking for barriers.
    - An alternative or supplement to dropdowns is a list of relevant entries per document.

- Footnotes and comments:

    - Footnotes are only understandable with their context. When displayed in a separate list, they must be linked on both sides (as with TEI Publisher).
    - Footnotes in the dropdown have the context but the same problems as with index annotations.
    - Editorial comments with a lemma are also understandable without a primary text.

- Underlining, additions, deletions, superscripts

    - Avoiding the interpretation of markup and simply reproducing it visually can make it invisible.

- Parallel texts

    - Depending on the intention of the edition and the length of the parallel texts, tables or chapters are suitable.

- Competing hierarchies: Presentation in the digital edition vs. structure of the original document

## Challenges in navigation in digital editions

- Pagination for longer documents:

    - Each view is a document and needs its own title for identification.
    - Switching between views makes navigation opaque.

- Information content per screen

## Links

- [Web Content Accessibility Guidelines (WCAG) 2.1](https://www.w3.org/TR/WCAG21/){:target="\_blank"} with internationally valid recommendations from W3C
- [eCH-0059 Accessibility Standard](https://www.ech.ch/de/ech/ech-0059/3.0){:target="\_blank"} for public authorities and licensed companies in Switzerland
- [Accessibility in the CMS of the University of Zurich](https://t.uzh.ch/access){:target="\_blank"} with various links to instructions and tools
- [Handouts of the Centre for Digital Editions ZDE Zurich](https://www.zde.uzh.ch/de/offers/handout.html)
