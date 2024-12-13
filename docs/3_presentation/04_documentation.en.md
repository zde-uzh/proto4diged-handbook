# 3.3 Documentation

**The purpose of DSE documentation** is to provide users with general, philological and technical information and to facilitate or simplify the subsequent use of the DSE. For users and subsequent users, it is made clear how the edition data was created, who created it, when it was created, where it was created and why it was created. The University Library of Zurich provides a good overview of data reuse [here](https://www.ub.uzh.ch/de/wissenschaftlich-arbeiten/mit-daten-arbeiten/daten-dokumentieren.html){:target="\_blank"}.

The DSE documentation is a central component of a DSE, which is why the time of its creation should be recorded in the project plan and the **documentation responsibilities** in the project team as early as the **planning phase**. If possible, there should be one main person responsible for the documentation, who collates the individual aspects (see below) from the relevant specialists.
During the planning phase, it should also be clarified **how detailed and in which data format** the documentation must be (see below), as the documentation ideally takes place during the documented work processes and only requires minimal editorial revision at the end.

In the following, we refer in detail to the [Documentation of the Showcase Edition](), which repeats many of the explanations in this manual (in particular the editing guidelines regarding transcription, annotation and commentary).

It should be noted that standardised documentation structures or designations for aspects of the documentation have only been established to a limited extent to date; this sometimes makes it difficult to compare the documentation. Standardisation would be desirable, but this chapter is not intended as a proposal in this regard, but rather an attempt to think about documentation in terms of (necessary and desirable) requirements.

## What does DSE documentation contain?

DSE documentation replaces the **editorial commentary** of a printed edition (which usually briefly explains the basics of the text constitution and the editorial guidelines) or its **editorial afterword** (which also explains the historical background of the edition and philological aspects).

The **Editionsmodell** of the DSE documentation supplements these classic editorial explanations with its **Guidelines for the creation of text-critical and content-related annotations and comments** in TEI/XML. In other words, it explains which coding is used for which forms of annotation and commentary in TEI/XML. The DSE is thus documented not only as an edition (philological), but also as a code (technical), whereby these two aspects are inextricably interwoven.
=> [Edition model of the showcase edition]()

The DSE documentation therefore also documents digital aspects that have no equivalent in print:

-   All **used tools** and the reason for their choice, ideally with a reference to their own documentation and, if applicable, their possible uses;
    => [Tool documentation of the showcase edition]()

-   the **origin of the digital resources**, e.g. external IIIF servers/platforms such as [e-manuscripta](https://www.e-manuscripta.ch/) or metadata sources (in addition to the **origin of physical sources**, i.e. the _digitised resources_, e.g. an archive);
    => [Resource documentation of the showcase edition]()

-   the **data model**, which in turn contains the **format of the data** and the **structuring of metadata**, ideally with explanations of where data standards are involved or where and why it was necessary to deviate from them;
    => [Data model of the showcase edition]()

-   the **measures for long-term preservation**, both regarding the [_functional edition with frontend_](../4_longterm_preservation/02_static_presentation.en.md) and the [_data_archiving_](../4_longterm_preservation/03_archiving_data.en.md) on other platforms with corresponding links to these resources.
    => [Long-term preservation documentation of the showcase edition]()

## Accessibility and presentation

Depending on the size, complexity and innovative content of a DSE, **different requirements** may have to be met by a DSE documentation, but it should fulfil certain basic requirements in its presentation:
It should be **recognisable** as documentation and be provided at the same level as the list of edited texts, the index or the search functions.

We generally recommend clearly separating the **sub-topics** of a documentation into technical, philological and organisational topics. The latter, general information on the project structure can also be presented outside the documentation (e.g. as a [_project entry page_](../3_presentation/02_access.en.md) about the institutions, team or funding involved). Rather **not part of the documentation** is background information on the edited content (as a scientific supplement in the sense of [_overview comments_](../2_Editionsarbeit/06_commenting.en.md)). **Citation suggestions** can be included in the documentation, but the minimum requirement is, as already mentioned, to display a clearly visible citation suggestion for each distinct page. It should not be necessary to consult the documentation to cite a DSE.

## Documentation types

The **minimum requirement for documentation** is a keyword-like explanation of all visible/usable components of the DSE.
DSE and thus corresponds more to the editorial commentary in print. The various aspects can be separated by simple sub-chapters and combined on a single page, which makes it easy to generate a PDF. This may be sufficient for a smaller or less complex DSE, especially if it continues a previous practice - in this case it is advisable to refer to the [_exemplary DSE_](../1_Planung/01_Projektziele_und_-ressourcen.en.md) in your own documentation.

!!! info "Exemplary DSE: Minimal documentation"
The [Digital Edition of the Travel Diaries of Johann Conrad Fischer 1794-1851](https://johannconradfischer.com/de/content/editorial-guidelines){:target="\_blank"} is a visually appealing DSE of a printed corpus that has already been critically edited in book form, which now primarily utilises the advantages of simple linking and visual enrichment. As it is based on established functions of the TEI Publisher, the documentation is content with minimal information on [Edition history and technology](https://johannconradfischer.com/de/content/about){:target="\_blank"} and the [Edition guidelines](https://johannconradfischer.com/de/content/editorial-guidelines){:target="\_blank"}.

In contrast, **extensive documentation** has more the character of an editorial epilogue and is divided into several subpages for better clarity. The more a DSE project is intended to be a role model within a community and/or the more innovative a DSE project is, the more detailed the documentation should be.

!!! info "Exemplary DSE: Detailed documentation"
Two DSEs are presented below that are 'haute couture' editions in technical terms and have correspondingly detailed documentation.

    The DSE [**Der Sturm**](https://sturm-edition.de/index.html){:target="\_blank"} brings together and edits a large number of very different documents relating to the international avant-garde of the 20th century. This makes various complex editorial guidelines etc. necessary. It has a detailed and clearly structured documentation of its [digital methodology](https://sturm-edition.de/projekt/methodik.html){:target="\_blank"}, its [TEI/XML coding](https://sturm-edition.de/edition.html){:target="\_blank"} and its [data resources](https://sturm-edition.de/ressourcen/schnittstellen.html){:target="\_blank"} (including interface for own data access).

    The previously mentioned letter correspondence DSE [**hallernet**](https://hallernet.org/){:target="\_blank"} is one of the most ambitious projects of recent years in terms of its database. This is also reflected in its [documentation](https://docs.hallernet.org/){:target="\_blank"}. A separate subdomain was created for this, almost exclusively in English, which contains three main categories (Guidelines/System/Usage) with subchapters. Particular attention is paid to the data model of the metadata. The documentation is primarily aimed at a technically and philologically savvy audience.

## Tools and data formats

**Use of TEI/XML**

DSEs can write their documentation in the **same data format**, usually TEI/XML, as the edited text. This makes sense if the documentation is to be published with the same tool, such as TEI Publisher. However, it should be noted that TEI/XML is a more complex data format than is normally required for documentation and, unlike Markdown (see below), is not a fixed standard but allows more flexibility. This is particularly relevant if parts of the documentation are written by employees who are not involved in the editing process themselves (e.g. technical employees who are responsible for the front end or long-term backup) and would therefore have to familiarise themselves with TEI/XML for this purpose alone (or their files have to be converted).

Conclusion: In small teams that are familiar with TEI/XML, the TEI/XML data format and associated tools make sense. A simplified XML alternative, which is used in the TEI Publisher documentation, for example, is the [DocBook XML](https://docbook.org/) format.

**Use of Markdown, e.g. together with MKDocs or vitepress**

Markdown is a data standard for technical documentation and therefore offers sufficient functionality for DSE documentation. There are also various freely accessible Python libraries that allow more complex documentation to be written with relatively simple means. One such Python library, [MkDocs](https://www.mkdocs.org/){:target="\_blank"} was used for this manual.

The [documentation of hallernet](https://docs.hallernet.org/){:target="\_blank"} (see above) is Markdown-based and is generated automatically in a CI workflow using a common tool for creating documentation ([vitepress](https://vitepress.dev/){:target="\_blank"}).

Markdown files can ultimately be **published** in various ways. For projects that use the TEI Publisher, it can be useful to publish their Markdown files directly in the Publisher, as explained in more detail in the [TEI Publisher documentation](https://teipublisher.com/exist/apps/tei-publisher/about.md?view=div){:target="\_blank"} is explained in more detail.

## Archiving of documentation

For the complete [_archiving of DSE_](../4_longterm_preservation/03_archiving_data.en.md) in repositories, the documentation can also be stored as a separate file (e.g. PDF), such as [here in swissubase](https://www.swissubase.ch/de/catalogue/studies/20701/19845/datasets/2556/3065/overview){:target="\_blank"}.
