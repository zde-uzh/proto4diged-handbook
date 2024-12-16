# 3.2 Views for the edition

The centrepiece of every DSE is the presentation of the edited text. The DSE community seems to have agreed on the minimum standards (two-part layout and XML downloads) in recent years, but there are other view and download functions that are also discussed below.

## The two-part layout

A **two-part layout** has established itself as the standard view, consisting of the transcribed and annotated text on the one hand and the rotatable and enlargeable digital copy on the other. The advantage of this view is that relationships between the source and the scientifically prepared text become immediately recognisable; this is also referred to as **autoptical comparison**. While print editions as historical-critical editions, which generally did without facsimiles, still had to make text-genetic complexity comprehensible with the help of a text-critical apparatus, the two-part digital layout simplifies the identification of foreign hands, subsequent corrections, postmarks or paratextual additions. Although these can still be identified in the transcribed text by means of annotations, DSEs can weigh up more freely what should be identified by the users and what should be additionally labelled, as the information of the source material is not lost in the editing process.

The autoptic comparison and thus the relationship between the digitised material and the transcription text can be supported by displaying graphic elements on the facsimile. As this is a presentation function that must already be prepared when the transcriptions are created (i.e. coordinates must be available at data level), we have already introduced the **linking of digitised material and transcriptions** in the subchapter [_transcription_](../2_Editionsarbeit/03_Transkription.en.md).

!!! info "Exemplary DSE: Linking digitised material and transcription"
    
    There is a best practice for this link in the [Escher-Briefedition](https://www.briefedition.alfred-escher.ch/home.html). However, it should be noted that the Escher-Briefedition requires the decision to present either the two-part layout with digitised text and diplomatic transcription or a one-part presentation with the annotated text ("Edited text (with index entries)"). On the one hand, this leads to greater clarity because the indexes can be clearly displayed on the page in the presentation of the annotated text. On the other hand, this solution can be criticised because the annotation and the digitised text cannot be viewed at the same time. The example shows the typical conflict between clarity and information density that occurs at various points in the presentation of DSE.

    ![alt text](../2_Editionsarbeit/image-3.png) <figcaption>[Jung Joseph (ed.), Digitale Briefedition Alfred Escher, Relaunch January 2022, Zurich.](https://briefedition.alfred-escher.ch/briefe/B0056?view1=1){:target="\_blank"} Retrieved on 22.9.2024. </figure>

## Reading versions

In addition to the digital copy and the transcribed and annotated text, many DSEs also offer a **reading version** that is based on the diplomatic transcription (see [_transcription_](../2_Editionsarbeit/03_Transkription.en.md)) but has undergone **normalisation**. This means that errors in the original text, incongruent or historical spellings and text-critical annotations such as deletions or underlining are corrected according to clearly defined editorial guidelines or brought closer to the spelling used in print today. Errors are erased, spellings are modernised and standardised, text-critical annotations are omitted or simplified (deletions are omitted, underlining is changed to italics). In addition, line breaks are variably adapted to the screen size and no longer correspond to the line breaks of the digital copy (exceptions: verses, drama texts, etc.).

The reading version can either be based on a new XML file at data level, or the XML file of the diplomatic transcription can be read out differently using the ODD. For the second option, it is necessary to annotate the correct word variants for the reading version at the latest during the content annotation in the event of corrections.

At the technical level of coding, a single-source principle is preferable when creating the reading version, i.e. the diplomatic version and the reading version result from the differentiation of the "mode" with which an ODD reads out a single XML (= single source). In simple terms, the read version is then a preselection of choice elements and an omission of breaks. With dropdowns in TEI Publisher, a read version can also be combined by selecting different display options.

## Multi-part, variable layouts

The **presentation of the reading version** can either be displayed on its own (similar to the presentation of the annotated text in the Escher edition described above) or combined with other views in a **two-part, three-part or multi-part layout**.

!!! info "Sample DSE: Two-part layout"
    
    The [Lokalbericht Edition](https://www.lokalbericht.ch/synopsis/LB.TEIL1.0010-d/LB.TEIL1.0010-d) is an example of a one- or two-part view. In contrast to the Escher letter edition, the "parallel view" allows you to choose whether the two parts consist of a digital copy, a transcription or a reading version of a page. In the "Synopsis" view, it is also possible to combine two different digital copies or to display a reading version with a digital copy belonging to another page.

    ![Views Lokalbericht](image.png) <figcaption>[Hermann Burger: Lokalbericht. Digital edition.](https://www.lokalbericht.ch/parallel/LB.TEIL1.0010-d/LB.TEIL1.0010-t){:target="\_blank"} Retrieved on 22.9.2024.</figure>

Here, too, it is important to weigh up how much **visual and conceptual complexity** DSE users should be expected to accept. This starts with the default setting of the view, but above all concerns the selection of how many views are possible. Not every possible display is actually useful for users.

!!! info "Exemplary DSE: Multi-part layout"

    An extreme example of a multi-part edition view is the edition portal of the German Literature Archive Marbach [Edview](https://edview.dla-marbach.de/). Edview is not structured like a conventional website, but in the style of a web-based desktop, which opens 'windows' within the browser and offers the user many configuration options.

    The entry point is already complex here, where several editions can be selected for research. In the actual edition view, texts from different editions can be displayed simultaneously in several windows. One to four windows are visible, each new view type (XML, facsimile, edition text, commentary, etc.) creates a new window and moves already open windows to the left into a non-visible area. The number of windows that can be selected for viewing using thumbnail icons appears to be unlimited. Windows can also be added to a virtual clipboard for later use.

    ![Edview Editionsansicht](image-1.png) <figcaption>[Harry Graf Kessler. Das Tagebuch 1880-1937, online edition 2024.](https://edview.dla-marbach.de/){:target="\_blank"} Retrieved on 22.9; linking specific view configurations is not possible in Edview. </figure>

## Download the text data: XML, JPG, PDF, ebooks

DSEs now often offer simple options for downloading different edition data directly from the edition view (instead of retrieving it from a repository for long-term archiving, for example). The XML file download function is standard, but interesting offers also include JPGs or PDFs of the digitised version as well as PDFs of the diplomatic transcription or the reading version. The option of downloading reading versions as ebooks (in the typical epub or mobi format) is still rare. This may be due to the fact that ebooks have so far hardly established themselves as a scientific working tool. However, this may change in the future if the technical functions already available in ebooks today (e.g. linking endnotes) become more widespread

!!! info "Exemplary DSE: Downloads"
    
    The (Missiven edition)[https://missiven.stadtarchiv.ch/index.html] of the St. Gallen City Archives and the Vadian Collection is created with the TEI Publisher and offers the download of XML, JPG and PDF data of each missive.
    
    ![Download options for missives edition](image-2.png) <figcaption> [Download options for the DSE "Briefverkehr der Stadt St. Gallen 1400-1650. Digitale Missivenedition"](<https://missiven.stadtarchiv.ch/namen/Brandenburg,%20Friedrich%20I.%20von%20(1438%E2%80%93)?&category=B&search=&key=stadtasg-actors-240>){:target="\_blank"}. Retrieved on 24.9.2024.</figure>

## Citation suggestions

Each DSE page (primarily from the edition, but ideally also from the documentation and from various commentary forms) should have a clearly visible reference\*\* as to how this page should be cited. Central components of the citation proposal are the names of the editors, the project and the version of the DSE cited at the specified time (if a version is available). It is advisable to use classic bibliography nomenclature as a guide.

## Licensing of the data

In order to make the data available as ORD (open research data), links to the data should be provided as standard wherever possible. This involves licensing the data as [creative commons](https://creativecommons.org/share-your-work/) or indicating what users may do with copyrighted data. The Centre for Digital Editions at UZH ZDE offers a [handout](https://www.zde.uzh.ch/de/offers/handout.html) with recommendations on open access and an overview of the legal basis in Switzerland.
