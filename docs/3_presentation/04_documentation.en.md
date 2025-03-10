# 3.3 Documentation

The **purpose of DSE documentation** is not only to provide general, philological, and technical information for users but also to enable and simplify the subsequent reuse of the DSE. For both users and future users, it should be clear how the edition data was created, who created it, when it was created, where it was created, and why it was created. The University Library of Zurich offers a useful overview of data reuse [here](https://www.ub.uzh.ch/de/wissenschaftlich-arbeiten/mit-daten-arbeiten/daten-dokumentieren.html){:target="\_blank"}.

DSE documentation is a central component of a DSE, which is why the time of its creation should be recorded in the project plan, along with the **documentation responsibilities** within the project team, starting in the **planning phase**. If possible, one person should take primary responsibility for the documentation, gathering the individual aspects (see below) from the relevant specialists. 
During the planning phase, it should also be determined **how detailed and in which data format** the documentation needs to be (see below), as the documentation ideally occurs during the work processes themselves, requiring only minimal editorial revision at the end.

In the following sections, we refer in detail to the [Documentation of the Showcase Edition](), which reiterates many of the explanations in this manual (particularly the editorial guidelines regarding transcription, annotation, and commentary).

It should be noted that standardized documentation structures or terms for documentation aspects have only been partially established to date; this sometimes makes it difficult to compare different documentation practices. While standardization would be desirable, this chapter is not intended as a proposal for such a standard, but rather as an attempt to conceptualize documentation in terms of (necessary and desirable) requirements.

## What Does DSE Documentation Contain?

DSE documentation replaces the **editorial commentary** of a printed edition (which typically provides a brief explanation of the basics of text constitution and editorial guidelines) or its **editorial afterword** (which additionally explains the historical background of the edition and philological aspects).

The **edition model** of DSE documentation complements these traditional editorial explanations with its **guidelines for the creation of text-critical and content-related annotations and comments** in TEI/XML. In other words, it clarifies which coding is used for different forms of annotation and commentary in TEI/XML. The DSE is therefore documented not only as an edition (philologically) but also as a code (technically), with these two aspects being inseparably intertwined.
=> [Edition model of the showcase edition]()

Thus, the DSE documentation also encompasses digital aspects that have no equivalent in print, such as:

-   all **tools involved** and the justification for their choice, ideally with a reference to their own documentation and, if applicable, their possible uses;
    => [Tool documentation of the showcase edition]()

-   the **origin of the digital resources**, e.g. external IIIF servers/platforms such as [e-manuscripta](https://www.e-manuscripta.ch/) or metadata sources (in addition to the **origin of physical sources**, i.e. the _digitized resources_, e.g. an archive);
    => [Resource documentation of the showcase edition]()

-   the **data model**, which in turn contains the **format of the data** and the **structuring of metadata**, ideally with information on where to find data standards or where and why it was necessary to deviate from them;
    => [Data model of the showcase edition]()

-   the **measures for long-term preservation**, both regarding the [_functional edition with front end_](../4_longterm_preservation/02_static_presentation.en.md) and the [_data_archiving_](../4_longterm_preservation/03_archiving_data.en.md) on other platforms with corresponding links to these resources.
    => [Long-term preservation documentation of the showcase edition]()

## Accessibility and Presentation

Depending on the size, complexity, and innovative content of a DSE, **different requirements** may need to be met by DSE documentation, but it should fulfil certain basic requirements in its presentation:
It should be recognizable as documentation and provided alongside the list of edited texts, the index, or the search functions.

We generally recommend clearly separating the categories of documentation into technical, philological, and organizational topics. General information on the project structure can also be presented outside the documentation (e.g., as a
[_project entry page_](../3_presentation/02_access.en.md) about the institutions, team, or funding involved). Background information on the edited content is generally **not part of the documentation** (such as scientific supplements in the form of [_overview comments_](../2_Editionsarbeit/06_commenting.en.md)). **Citation suggestions** can be included in the documentation, but the minimum requirement is, as already mentioned, to provide a clearly visible citation suggestion for each distinct page. It should not be necessary to consult the documentation in order to cite a DSE.

## Documentation Types

The minimum requirement for documentation is a brief, keyword-like explanation of all visible/usable components of the DSE, which corresponds more to the editorial commentary in a printed edition. The various aspects can be separated into simple sub-chapters and combined on a single page, making it easy to generate a PDF. This may be sufficient for a smaller or less complex DSE, especially if it continues a previous practice. In this case, it is advisable to refer to the [_exemplary DSEs_](../1_Planung/01_Projektziele_und_-ressourcen.en.md) in your own documentation.

!!! info "Example DSE: Minimal Documentation"
    
    The [Digital Edition of the Travel Diaries of Johann Conrad Fischer 1794–1851](https://johannconradfischer.com/de/content/editorial-guidelines){:target="\_blank"} is a visually appealing DSE of a printed corpus that has already been critically edited in book form, now primarily utilizing the advantages of simple linking and visual enrichment. Since it is based on established functions of the TEI Publisher, the documentation only provides minimal details about [Edition history and technology](https://johannconradfischer.com/de/content/about){:target="\_blank"} and the [Edition guidelines](https://johannconradfischer.com/de/content/editorial-guidelines){:target="\_blank"}.

In contrast, an **extensive documentation** has more of the character of an editorial afterword and is divided into several subpages for better clarity. The more a DSE project is intended to serve as a role model within a community and/or the more innovative a DSE project is, the more detailed the documentation should be.

!!! info "Example DSE: Detailed Documentation"

    Two DSEs are presented below that are 'haute couture' editions in technical terms and feature correspondingly detailed documentation.

    The DSE [**Der Sturm**](https://sturm-edition.de/index.html){:target="\_blank"} brings together and edits a wide variety of very different documents related to the international avant-garde of the 20th century. This requires various complex editorial guidelines, etc. It features detailed and clearly structured documentation of its [digital methodology](https://sturm-edition.de/projekt/methodik.html){:target="\_blank"}, its [TEI/XML coding](https://sturm-edition.de/edition.html){:target="\_blank"} and its [data resources](https://sturm-edition.de/ressourcen/schnittstellen.html){:target="\_blank"} (including an interface for accessing its own data).

    The previously mentioned letter correspondence DSE [**hallernet**](https://hallernet.org/){:target="\_blank"} is one of the most ambitious projects of recent years in terms of its database. This is also reflected in its [documentation](https://docs.hallernet.org/){:target="\_blank"}. A separate subdomain, almost exclusively in English, was created for this, which contains three main categories (Guidelines/System/Usage) with subchapters. Particular attention is paid to the data model of the metadata. The documentation is primarily aimed at a technically and philologically sophisticated audience.

## Tools and Data Formats

**Use of TEI/XML**

DSEs can write their documentation in the **same data format**, usually TEI/XML, as the edited text. This is useful if the documentation is to be published with the same tool, such as TEI Publisher. However, it should be noted that TEI/XML is a more complex data format than is typically required for documentation and, unlike Markdown (see below), it is not a fixed standard but offers more flexibility. This is particularly relevant when parts of the documentation are written by employees who are not involved in the editing process (e.g., technical staff responsible for the front end or long-term preservation) and would, therefore, need to familiarize themselves with TEI/XML solely for this purpose (or their files would need to be converted).

Conclusion: In small teams familiar with TEI/XML, the TEI/XML data format and associated tools are a good choice. An alternative simplified XML format, used in TEI Publisher documentation, for instance, is [DocBook XML](https://docbook.org/).

**Use of Markdown, e.g., with MKDocs or VitePress**

Markdown is a data standard for technical documentation and, therefore, provides sufficient functionality for DSE documentation. Additionally, there are several freely accessible Python libraries that allow more complex documentation to be created with relatively simple tools. One such Python library, [MkDocs](https://www.mkdocs.org/){:target="\_blank"}, was used for this manual.

The [documentation of hallernet](https://docs.hallernet.org/){:target="\_blank"} (see above) is Markdown-based and is automatically generated in a CI workflow using a common tool for creating documentation ([VitePress](https://vitepress.dev/){:target="\_blank"}).

Markdown files can ultimately be **published** in various ways. For projects that use the TEI Publisher, it may be useful to publish their Markdown files directly in the Publisher, as explained in more detail in the [TEI Publisher documentation](https://teipublisher.com/exist/apps/tei-publisher/about.md?view=div){:target="\_blank"}.

## Archiving of Documentation

In the context of the overall [_archiving of DSE_](../4_longterm_preservation/03_archiving_data.en.md)  in repositories, the documentation can also be stored as a separate file (e.g., PDF), such as [here in SWISSUbase](https://www.swissubase.ch/de/catalogue/studies/20701/19845/datasets/2556/3065/overview){:target="\_blank"}.
