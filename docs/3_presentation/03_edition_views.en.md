# 3.2 Edition Views

The core of any DSE is the presentation of the edited text. In recent years, the DSE community has largely agreed on minimum standards - namely, a two-part layout and XML downloads - but additional viewing and download options are also worth discussing.

## The Two-Part Layout

A **two-part layout** has become the standard, consisting of the transcribed and annotated text on one side and an interactive, rotatable, and zoomable facsimile on the other. This format makes the relationship between the original source and the scholarly edited text immediately visible - an approach known as **autoptic comparison**. While print editions, as historical-critical editions that generally did without facsimiles, still had to make the textual development comprehensible with the help of a text-critical apparatus, the two-part digital layout simplifies the identification of foreign hands, subsequent corrections, postmarks, or paratextual additions. While these features can still be highlighted in the transcription through annotations, DSEs have greater flexibility in deciding what should be explicitly marked and what can be left for users to discover, as no information from the original source is lost in the digital editing process.

The autoptic comparison between the facsimile and the transcription can be enhanced by overlaying graphical elements directly on the digitized image. Since this requires precise coordinate data, the groundwork for this feature must be laid during the transcription process. We have already introduced the **linking of facsimiles and transcriptions** in the [_transcription_](../2_Editionsarbeit/03_Transkription.en.md) subchapter.

!!! info "Example DSE: Linking Digitized Material and Transcription"

    The Alfred Escher Letter Edition provides a best-practice example of this type of linking. However, it requires users to choose between a two-part layout - featuring the digitized document alongside its diplomatic transcription - or a single-page view displaying the annotated text ("Edited text (with index entries)"). On the one hand, this improves clarity, as the index entries can be prominently displayed alongside the annotated text. On the other hand, a drawback of this approach is that the annotations and the digitized text cannot be viewed simultaneously. This example illustrates the typical trade-off between clarity and information density that arises in various aspects of DSE presentation.

    ![alt text](../2_Editionsarbeit/image-3.png) <figcaption>[Jung Joseph (ed.), Digitale Briefedition Alfred Escher, Relaunch January 2022, Zurich.](https://briefedition.alfred-escher.ch/briefe/B0056?view1=1){:target="\_blank"} Accessed on 22.9.2024. </figure>

## Reading Versions

In addition to the digital facsimile and the transcribed and annotated text, many DSEs also offer a **reading version** based on the diplomatic transcription (see [_Transcription_](../2_Editionsarbeit/03_Transkription.en.md)) but with **normalization** applied. This means that errors in the original text, inconsistent or archaic spellings, and text-critical annotations such as strikethroughs or underlining are corrected according to clearly defined editorial guidelines or adjusted to align with modern print conventions. Errors are removed, spellings are modernized and standardized, and text-critical annotations are either omitted or simplified (e.g., strikethroughs are removed, and underlining is converted to italics). Additionally, line breaks are dynamically adjusted to fit the screen size rather than following the original layout of the facsimile (exceptions include verse, dramatic texts, and similar formats).

At the data level, the reading version can either be based on a separate XML file or generated dynamically from the XML of the diplomatic transcription using ODD. In the latter case, any necessary corrections must be annotated with the appropriate word variants for the reading version during content annotation.

From a technical perspective, a single-source approach is preferable when generating the reading version. This means that both the diplomatic and reading versions are derived from the same XML file, with the difference determined by the mode in which the ODD processes the document. Simply put, the reading version is a preselection of choice elements with omitted line breaks. In TEI Publisher, dropdown menus can allow users to customize the reading version by selecting different display options.

## Multi-Part, Flexible Layouts

The **presentation of the reading version** can either be displayed on its own (similar to the presentation of the annotated text in the Escher Edition described above) or integrated into a **two-part, three-part, or multi-part layout** alongside other views.

!!! info "Example DSE: Two-part Layout"
    
    The [Lokalbericht Edition](https://www.lokalbericht.ch/synopsis/LB.TEIL1.0010-d/LB.TEIL1.0010-d) offers both single- and two-panel viewing options. Unlike the Escher Letter Edition, its "parallel view" allows users to freely choose whether the two panels display a facsimile, a transcription, or a reading version of a page. The "synopsis" view even makes it possible to combine two different facsimiles or to display a reading version alongside a facsimile from a different page.

    ![Views Lokalbericht](image.png) <figcaption>[Hermann Burger: Lokalbericht. Digital edition.](https://www.lokalbericht.ch/parallel/LB.TEIL1.0010-d/LB.TEIL1.0010-t){:target="\_blank"} Retrieved on 22.9.2024.</figure>

Here, too, it is crucial to consider how much **visual and conceptual complexity** can be reasonably expected from DSE users. This applies not only to the default view settings but also to the overall selection of available views. Not every technically possible configuration is necessarily useful or practical for users.

!!! info "Example DSE: Multi-part Layout"

    An extreme example of a multi-part edition view is the edition portal of the German Literature Archive Marbach, [Edview](https://edview.dla-marbach.de/). Edview is not structured like a conventional website but in the style of a web-based desktop, which opens 'windows' within the browser and offers users many configuration options.

    The entry point itself is already complex, as multiple editions can be selected for research. In the actual edition view, texts from different editions can be displayed simultaneously in several windows. One to four windows are visible, and each new view type (XML, facsimile, edition text, commentary, etc.) generates a new window, moving already open windows into a non-visible area to the left. The number of windows that can be selected for viewing using thumbnail icons seems unlimited. Windows can also be added to a virtual clipboard for later use.

    ![Edview Edition View](image-1.png) <figcaption>[Harry Graf Kessler. Das Tagebuch 1880-1937, online edition 2024.](https://edview.dla-marbach.de/){:target="\_blank"} Retrieved on 22.9; linking specific view configurations is not possible in Edview. </figure>

## Downloading Text Data: XML, JPG, PDF, eBooks

DSEs now often offer easy options for downloading various edition data directly from the edition view (instead of retrieving them from a long-term archiving repository, for example). The download of the XML file is the standard feature, but interesting options also include JPGs or PDFs of the digitized version, as well as PDFs of the diplomatic transcription or the reading version. The option to download reading versions as eBooks (in the typical EPUB or MOBI format) is still rare. This may be because eBooks have not yet established themselves as a significant scientific tool. However, this could change in the future if technical functions already available in eBooks today (such as linking endnotes) become more widespread.

!!! info "Example DSE: Downloads"
    
    The (Missiven edition)[https://missiven.stadtarchiv.ch/index.html] of the St. Gallen City Archives and the Vadian Collection is created with the TEI Publisher and offers the download of XML, JPG, and PDF data for each missive.
    
    ![Download options for the Missiven edition](image-2.png) <figcaption> [Download options for the DSE "Briefverkehr der Stadt St. Gallen 1400-1650. Digitale Missivenedition"](<https://missiven.stadtarchiv.ch/namen/Brandenburg,%20Friedrich%20I.%20von%20(1438%E2%80%93)?&category=B&search=&key=stadtasg-actors-240>){:target="\_blank"}. Retrieved on 24.9.2024.</figure>

## Citation Suggestions

Each DSE page (primarily from the edition, but ideally also from the documentation and various forms of commentary) should include a **clearly visible reference** indicating how the page should be cited. Key components of the citation suggestion are the names of the editors, the project, and the version of the DSE cited at the specified time (if a versioning system is in place). It is recommended to follow standard bibliographic conventions as a guide.

## Licensing of the Data

To provide the data as ORD (open research data), links to the data should be offered as a standard wherever possible. This involves licensing the data under [creative commons](https://creativecommons.org/share-your-work/) and indicating what users are permitted to do with copyrighted data. The Centre for Digital Editions at UZH ZDE offers a [handout](https://www.zde.uzh.ch/de/offers/handout.html) with recommendations on open access and an overview of the legal framework in Switzerland.
