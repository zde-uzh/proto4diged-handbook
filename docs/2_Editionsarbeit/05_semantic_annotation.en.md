# 2.4 Content Annotation

## What is Digital Content Annotation?

By _content annotation_ we mean the labelling of a word or word sequence with regard to its **semantic references**. These can refer to the same text (intratextual), other texts/works (intertextual), or any facts (contextual). This chapter will primarily deal with inter- and contextual referencing, as these are the most challenging both in terms of editorial research effort and the technical tools and interfaces required. Nevertheless, projects should not ignore intratextual references, as they make navigation within a larger text much easier.

Common examples:

-   Intratextual content annotations:

    -   Referencing a letter appendix within a letter passage.
    -   Referencing chapters within a table of contents.

-   Intertextual content annotations:

    -   Linking a reference to a work (discussed in a letter) to a bibliographic entry in the DSE register or a library database—or ideally, to a [_standard database_](../Themen/authority.en.md).
    -   Connecting a passage in one text to another text within the same DSE, or to a text edited in a different DSE.

-   Contextual content annotations:
    -   Linking a text passage to an entry in the DSE's own gazetteer or a geographical database like [geonames.org](https://www.geonames.org/).
    -   Connecting a text passage to an entry in the DSE's own index of persons, or to a personal data standards database like the [Gemeinsame Normdatei (GND)](https://gnd.network/Webs/gnd/DE/Home/home_node.html).

In contrast to text-critical annotation, which is often done during the [_transcription_](03_Transkription.en.md) (see 3.5), a content-annotated text passage appears as a link that makes the reference accessible with a click (alternatively, it can also be identified through hover/mouseover text). Unlike [_commenting_](06_commenting.en.md), a content annotation is a **simple reference** that should be **self-explanatory** or, at the very least, explained by linking to a resource within the edition (e.g., an entry in an index or on a map) or to an external resource (e.g. a [_standard database_](../Themen/authority.en.md) such as [GND](https://gnd.network/Webs/gnd/EN/Home/home_node.html)).

Content annotation is an editorial task specifically enabled by digital tools, particularly the ability to create links. It produces the digital equivalent of a **book index** (e.g., a subject, name, or place index at the end of a scholarly edition), but with broader functions and greater completeness. The extensive interlinking of annotations with external digital resources supports the concept of [**Linked Open Data**](https://handbook.opendata.swiss/de/content/glossar/bibliothek/linked-open-data.html){:target="\_blank"}: the visualization, linking, sharing, and integration of openly accessible datasets.

## 1. Standard Solutions for Content Annotation

Content annotation is typically carried out using the same tool as commentary; a detailed examination of the digitized material is no longer absolutely necessary for both steps. Transcription tools like Transkribus currently do not offer these functions, meaning they do not yet allow for the creation of content annotations such as links or comments. These features are planned for implementation by the summer of 2024. However, if they are added, they should be used with caution, as each additional annotation function in the transcription tool may introduce new challenges in [_conversion_](04_converting.en.md) - at least until transcription tools gain the ability to [_publish_](../3_presentation/01_introduction_presentation.en.md) TEI/XML data independently.

There are two available standard technical solutions, and their workflows are documented in the next subchapter:

1. The use of a tool that allows both **editing and publishing**. The TEI-Publisher is a thoroughly tested solution for this purpose.

2. The use of a **TEI/XML editor** such as Oxygen, which serves as a bridge between the transcription tool and the publication tool.

## 2. Standard Workflow Steps

### 2.1 Creating the Editing Guidelines

Regardless of the tool used, it is essential to clarify at the outset which content needs to be annotated and for what purpose. The guiding question should be what usage scenarios the DSE is intended to fulfill:

- Should it collect as much content data as broadly as possible, or is the focus on very specific data?
- What specific data is needed in each case?

Over the past few years, five main categories of inter- and contextual references have emerged, as seen in the examples mentioned earlier: **personal data, location data, time data, work data, and keywords**. While work data and keywords are not found in every DSE, persons, places, and times have become standard.

A bit more unconventional is the referencing of other categories, for which there are virtually no technical limits, such as freely chosen topics (more specific than keywords), historical events, or linguistic features (e.g., the use of foreign languages).

!!! Warning "Challenge"

    From an editorial perspective, the expansion of categories is always associated with the problem that once a category is introduced, it must be applied consistently, which can become quite time-consuming. In the case of multiple editors, this requires strict adherence to complex editorial guidelines, or constant coordination for adjustments. Complex issues that only need to be made understandable in a few texts should therefore be addressed in the passage or text [_comment_](06_commenting.en.md).

When planning content annotation, the following editorial considerations should be taken into account:

- Is the DSE's own index central, for instance, because there are hardly any other datasets available on the internet for it?
- Or should the index, in most cases, serve as an 'intermediate stop' to consolidate information and link it to external resources?

Both standard tool solutions allow the **integration of connectors**, meaning the semi-automated linking of annotations in TEI-XML to a standards database. Editors can select the correct standards dataset from the connector's suggestions, eliminating the need to manually research and insert the link into TEI/XML. However, if the likelihood of finding any external standards data is low, the use of connectors becomes secondary.

It is important to carefully consider how frequently each type of data should be labelled in a text and which standards (see below) should be referenced for this purpose. For instance, it would not be practical to annotate salutations (e.g., you/your) in letters every time, especially if the person being addressed is the same as the recipient (since this information is already included in the letter's metadata). While such considerations may seem trivial, they should be incorporated into the editorial guidelines and made available to DSE users.

!!! abstract "Showcase Editing Guidelines: Content Annotation"

    Our project decided to annotate three categories: place, person, and work. In the case of Gaston Paris's historical scholarly correspondence, these categories are best suited for tracing the scholar's research network, which is central to the project leader's own research.

    - **Places** are linked to geonames using their current place names, where possible.
        - Places are not annotated if they already appear in the letter's metadata (such as the place of sending or receiving).

    - **Persons** are first linked to personal data in the GND (German National Library's integrated authority file). This is the simplest form of standard data linking, as the link to GND is preconfigured in the TEI Publisher. In a second step, a link will also be made to [VIAF](https://viaf.org/){:target="\_blank"}, an international aggregator of authority data, and to [IdRef](https://www.idref.fr/){:target="\_blank"}, the French standards database. IdRef is especially significant due to the French-language corpus and Romance studies focus, but as of 2024, it cannot yet be automatically linked to the TEI Publisher. Personal data that is not yet listed in the GND will be added via a service provided by the GND editorial team at the Zentralbibliothek Zürich, making it linkable. This contributes to improving GND records, particularly for French/Romance data.

        - Persons are not annotated in the text if they are already part of the metadata (author or recipient).

    - **Works** are imported from the project leader's extensive bibliography using the Zotero bibliography tool. The resulting index could be linked to work data from the GND in a second step, though this has not been implemented in the showcase edition.

#### Referencing Standardized Data

**Standardized vocabulary** in general, and the GND in particular, strengthens interoperability based on the FAIR principles. The GND, with its 10 million standardized records covering persons, geographies, corporate bodies, conferences, work titles, and subject terms, is freely available for reuse. While it was initially used mainly for cataloging materials in libraries, it is now increasingly being applied for cataloging collections in archives and museums, as well as in various digital project and research contexts such as DSEs. The resources cataloged in this way become compatible with modern search environments, while the use of controlled vocabulary enhances the retrievability and visibility of resources.

In the annotation process, collaborating with a specialized library service can help close the gap that editing projects often encounter ("some people who appear in the correspondence do not yet have a GND or VIAF entry", Sarah Rebecca Ondraszek: [Data, Data, there to Crawl, Who's the Fairest of Them All?](https://doi.org/10.58079/nkrq)). The [**GND editorial team of the University Library and Zurich Central Library**](https://www.zde.uzh.ch/de/analytics/openup.html) supports digital edition projects in actively using and independently entering data into the GND web form. The GND editorial team provides access and training on working with the web form, allowing the data entered to be immediately available in the GND and linked in the annotation. The team also offers an introductory guide to GND and provides advice on subsequent data reuse. In consultation, they check which persons, places, etc. from existing lists or registers are already in the GND.

For the Anglophone domain, the [**Library of Congress Subject Headings**](https://www.loc.gov/aba/cataloging/subject/) (LCSH) plays a central role in subject indexing, while for the Francophone domain, [**Répertoire d'autorité-matière encyclopédique et alphabétique unifié**](https://rameau.bnf.fr/) (RAMEAU) is key, especially via the Identifiants et référentiels (IdRef). The GND itself also links matching entities from these authority files. Furthermore, the collection [**VIAF**](https://viaf.org/) (Virtual International Authority File) brings together multiple authority files and Wikidata in a standardization data service hosted by OCLC. While the index link to the GND is directly integrated into the TEI Publisher, IdRef can only be accessed indirectly for annotation through aggregators or concordances.

### 2.2 Content Annotation in the TEI Publisher

Since version 7 (as of summer 2024: version 9), the open-source software [TEI Publisher](https://teipublisher.com/) has offered the option of enriching TEI/XML data with annotations using a graphical interface. This means that the text to be edited does not appear as TEI/XML and has to be edited as code but can be displayed similarly to the word processing program Word. However, the coding in TEI/XML can be checked at any time and also manipulated directly, which is sometimes necessary but requires additional expertise.

#### Choice of ODDs

Once the TEI/XML data has been imported into the TEI Publisher, it can be displayed on the tool's user interface using different ODDs (**O**ne **D**ocument **D**oes it all). ODD files (a detailed description can be found in the [Konde White Paper](https://www.digitale-edition.at/o:konde.150)) are written in the ODD schema language; they output the TEI/XML code based on different, defined schemas. In the case of the (here text-critical) annotation `<hi rend="underline">rassuré</hi>`, for example, the ODD 'recognizes' that the word "rassuré" should be underlined.
[The TEI consortium offers various ODDs and documents their use](https://tei-c.org/guidelines/customization/getting-started-with-p5-odds/); as TEI-XML is a flexible standard, not every annotation must and can be used for the same thing. In German-speaking countries, the [ODD of the German Text Archive](https://www.deutschestextarchiv.de/doku/basisformat/schema.html) has become established for editions in addition to the standard ODDs of the consortium. ODDs can be customized for each project, for example, using the online tool [ROMA](https://roma.tei-c.org/).
Technically, there are two different use cases for the ODD, the representation and the validation of the data; actually (i.e., according to the specification) both are intended as part of the same document, but in practice, the representation is often defined separately in the TEI Publisher environment.

#### Annotation Editor

The TEI Publisher has various standard ODDS pre-installed; the revision mode for annotation also has the form of an ODDS. This ODD has the file name 'annotations.odd' and can simply be selected from a page tab. The annotation editor activated by this can be customized, see the [TEI-Publisher documentation](https://teipublisher.com/exist/apps/tei-publisher/documentation/configuring-annotation-editor?action=search&view=div&odd=docbook.odd#3.42.13.63.3); we have also summarized important information in the subchapter [_Annotations with TEI-Publisher_](../Themen/tei-publisher-annotations.en.md).

!!! note "Experiences from the Showcase Edition"
    
    In order to activate all the required annotations in the edition editor, several attempts, meetings, and rounds of revision were necessary. Among other things, the project has recognized the need to display the digitized text, which is relatively small at the bottom of the screen in the annotation editor's default setting, in a larger format to the right of the annotated text. This means that text-critical annotations or corrections to the transcription, for which a comparison with the facsimile is necessary, can also be added. 
    The customized annotation ODD of the project is publicly available via GitLab:   
    => PASTE PROJECT RESOURCES HERE ![Annotations-Editor TEI Publisher](image-4.png)

The TEI Publisher stores all content annotation data in an **XML register**, where both standardization data IDs and your own generated data are stored. The use of an additional database is therefore unnecessary.

### 2.3 Content Annotation in Oxygen with and without Ediarum

After importing the TEI-XML data into the editor, the annotation is carried out using the [ediarum](https://www.ediarum.org) working environment. Ediarum displays TEI-XML data in a similar way to a Word file and has corresponding formatting buttons. Detailed ediarum [documentation](https://www.ediarum.org/docs.html) exists for [setting up](https://www.ediarum.org/docs/set-up/), [configuring](https://github.com/ediarum/ediarum.SKOS.edit?tab=readme-ov-file#installation) and [using](https://www.ediarum.org/docs/ediarum.BASE.manual) the editing environment and is regularly updated by the ediarum team.

=> This point is enriched by experience from the Schwarzenbach project, whereby the use of ediarum is probably limited to very few functions.

## 4 Limitations

The listed standard approaches for annotating content share the same **editorial limitation**: the more annotation categories are introduced into the edition, the harder it becomes to consistently follow the edition guidelines.

On the technical side, two primary limitations can be distinguished:

1. If a **user-friendly annotation interface** such as the TEI Publisher annotation editor or the ediarum extension for Oxygen is used, the easier operation comes with a limitation of annotation options. Expanding these options requires regular support from a technical expert and possibly more complex trial phases.

2. If an **XML editor** such as Oxygen is used, the introduction to coding work for annotation creation requires more effort; the editing environment is not 'ready to use,' and annotation must be practiced. However, extending and adapting the edition guidelines requires less technical support.

Which of the two paths requires less overall effort on the technical and editorial side depends on the **dynamics of the project's complexity**. If the edition guidelines for content annotation are simple and set from the start, the first approach is preferable. If the project is complex (e.g., due to a growing corpus that is initially hard to estimate), and the annotation requirements are difficult to define from the outset, working directly in the TEI/XML code is likely the more sensible option. The longer technical familiarization period for editing staff will then pay off in greater flexibility.
