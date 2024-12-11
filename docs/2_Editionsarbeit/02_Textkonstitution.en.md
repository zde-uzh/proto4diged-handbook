# 2.1 Constituting Texts (corpus selection and digitisation)

Text constitution refers to the compilation of the texts to be edited. If it is a text-genetically oriented edition, i.e. if the history of the creation and publication of a work is to be made comprehensible, the text constitution includes the **finding and selection of all text stages** to be edited (manuscripts or typescripts and proofs that were created in the creative process) and the **text editions** (various authorised or non-authorised prints, possibly also with handwritten notes or corrections by authors, editors and publishers).

At first glance, the edition-philological considerations in the text constitution appear to be independent of whether the intended edition is to be digital or printed. In fact, however, the location of the textual witnesses to be edited and their access and publication rights play a role, as different forms of publication (open/restricted/closed access, with or without digitisation) can result, as will be shown below.

## 1 Access to the text source and publication rights

The constitution of the text is linked to whether and how the physical **text sources for transcription are accessible** or can be made accessible. An edition may decide against editing text sources if they are difficult to access and involve a great deal of (financial, logistical or legal) effort. Text sources may even already be digitised and available on the database of a memory institution (see below) or [archive.org](https://archive.org/){:target="\_blank"}.

For DSE, further steps are part of the text constitution that decide on the edition of a text source, namely clarifications on the **legal modalities** of how the text sources are made available to the edition. The copyright holders or owners of a text source - the later by controlling access to it - can prohibit a digital, widely accessible publication of the digitised material and/or demand strong restrictions. In extreme cases, this can be a reason to refrain from publishing the text source altogether. However, attempts to comply with legal restrictions can also mean, for example, that the digitised copies of the text sources are only used in the work process and are not published or that texts and digitised copies are copy-protected.

!!! info "Exemplary DSE"
    [The online edition of Friedrich Dürrenmatt's Stoffe](https://fd-stoffe-online.ch/){:target="\_blank"} takes a legally restrictive approach : The digital copies can be displayed but not downloaded, the transcribed text only allows a copy of a certain number of characters and is not available as TEI/XML. This limited functionality, which deviates from now established DSE data and presentation standards, was analysed from an open access perspective in a [review of the journal RIDE](https://ride.i-d-e.de/issues/issue-17/duerrenmatt/){:target="\_blank"} (A review journal for digital editions and resources). The Stoffe project is an example of a compromise made early in the planning phase: the decision to make a legally protected text accessible at all can be accompanied by major restrictions.

## 2. Paths to the digitised text

Once legal issues have been clarified, institutional and technical questions arise in the digital text constitution, which have far-reaching consequences for long-term publication and preservation. We distinguish between three basic paths to digitisation, making it available and integrating it into the DSE.

**2.1 Digitisation and making available by a memory institution**

This is the desirable standard or _best practice_ on the path to digitisation: the memory institution (archive, library, museum, etc.) that owns the text source digitises it and makes it digitally accessible to the public itself. Digitisation is carried out according to established standards (e.g. [ISO standards](http://ikeep.com/ISO_14721){:target="\_blank"}) and in consistent quality. After the digitisation process, it is archived in a database by the memory institution for the long term.

Such public databases are usually operated by a network of memory institutions, e.g. in the canton of Vaud [Patrinum](https://patrinum.ch/?ln=fr){:target="\_blank"} or in German-speaking Switzerland [e-manuscripta](https://www.e-manuscripta.ch){:target="\_blank"}. There, the image data is made accessible with the [IIIF standard](https://www.digitale-edition.at/o:konde.123){:target="\_blank"}. This means that each document receives a IIIF-Manifest (describing the images of the digitised text within the document) and can be accessed via corresponding interfaces.

!!! note "Experience from the showcase edition"
    In the text constitution of Gaston Paris' exemplary letter edition, it was possible to draw on many years of research experience and an overview of the corpus. For a previous project, all of Gaston Paris' letters were digitised by the French National Library and made available online. It was therefore possible to quickly download [the relevant digital copies in their Gallica database](https://gallica.bnf.fr/ark:/12148/btv1b525187862){:target="\_blank"} could be downloaded for further processing.

    Due to download restrictions in Gallica, the images could not be accessed via the corresponding IIIF, which was not a problem given the small size of the project. In the case of larger quantities of images that need to be accessed via IIIF, we recommend contacting the database administration in such cases.

    A [GitLab page for the image metadata was created](https://gitlab.uzh.ch/digital-editions/proto4diged/image-metadata){:target="\_blank"} to ensure remote access to the image data for all project team members and to assign the pages to Transkribus and the TEI Publisher.

The great advantage of this approach is that the long-term storage of the image data is not in the hands of a temporarily limited project. This follows the **modular logic** of organising the operation and backup of the various DSE components independently of each other (see [_project goals and resources_](../1_Planung/01_Projektziele_und_-ressourcen.en.md)).

**2.2 Digitisation by a memory institution, making available through the project**

If the memory institution does not make the digitised material available on a database itself - either because it does not have such a database, because the selection is too small or too specific, or because the text source does not come from its own holdings - it is also possible to use a **IIIF server from another institution**. University libraries now often offer projects storage space on such a server at no extra cost. This additional financial outlay - like all other server costs - must be applied for beyond the duration of the project. In this case, the image data cannot be accessed independently via a database, but can be accessed independently via the Internet using a separate URI.

**2.3 Digitisation and backup by the project**

A **project's own digitisation** should be considered if access to a digitisation service is difficult (e.g. if the holdings are located in archives without a digitisation department and transport to another institution is not possible or does not make sense). The project's own digitisation can also be considered if the project manages the text sources itself, professional scanners are available and the digitisation work can be carried out by auxiliary assistants or similar. It is important that the work is planned and supervised by specialists and is  not carried out at the expense of research or editing time of academical employees (e.g. doctoral students or postdocs).
