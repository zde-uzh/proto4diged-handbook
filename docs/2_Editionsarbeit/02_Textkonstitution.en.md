# 2.1 Constitution of Text (Corpus Selection and Digitization)

The constitution of text refers to the compilation of texts to be edited. In the case of a text-genetic edition, i.e., if the creation and publication history of a work is to be reconstructed, the constitution of text includes the **identification and selection of all textual stages** to be edited (manuscripts, typescripts, and proofs that were produced in the course of the work's creation and development) as well as the **text editions** (various authorised or unauthorised prints, possibly annotated or corrected by authors, editors, or publishers).

At first glance, the edition-philological considerations in the constitution of text seem independent of whether the intended edition is to be digital or printed. However, the location of the textual witnesses to be edited and their access and publication rights do play a role, as they can determine the possible forms of publication (open/restricted/closed access, with or without digitisation), as will be demonstrated below.

## 1 Access to the Text Carrier and Publication Rights

The constitution of text is linked to whether and how **physical text carriers can be accessed for transcription**. An edition may decide against working with certain text carriers if they are difficult to access and involve significant (financial, logistical or legal) effort. In some cases, text carriers may already be digitized and available in the database of a memory institution (see below) or on [archive.org](https://archive.org/){:target="\_blank"}.

For DSE, additional steps of the constitution of text involve clarifying the **legal modalities** for how the text carriers will be made available in the edition. The rights holders or owners of a text carrier may prohibit a digital, widely accessible publication of the digitized material and/or impose strict restrictions (the latter not through copyright law, but by controlling access to the text carrier itself). In extreme cases, this can lead to a decision not to edit the text carrier at all. However, attempts to comply with legal restrictions can also mean that, for example, the digitized copies of the text carrier will be used only in the work process and will not be published, or that texts and digitized copies will be equipped with copy protection.

!!! info "Example DSE"
    
    [The online edition of Friedrich Dürrenmatt's _Stoffe_](https://fd-stoffe-online.ch/){:target="\_blank"} takes a legally restrictive approach : the digitized copies can be displayed but not downloaded, the transcribed text can only be copied up to a limited number of characters and is not available as TEI/XML. This restricted functionality, which deviates from now established DSE data and presentation standards, was analyzed from an open-access perspective in [RIDE](https://ride.i-d-e.de/issues/issue-17/duerrenmatt/){:target="\_blank"} (A review journal for scholarly digital editions and resources). The _Stoffe_-project exemplifies a compromise made early in the planning phase: the decision to make a legally protected text accessibleat all often comes with significant limitations.

## 2. Paths to the Digitized Copy

Once legal issues have been resolved, institutional and technical questions arise in the digital constitution of text, with far-reaching consequences for long-term publication and preservation. We distinguish three fundamental paths to digitization, its availability, and its integration into the DSE.

**2.1 Digitization and Access Provided by a Memory Institution**

This path represents the ideal standard or _best practice_ of digitization. The memory institution (archive, library, museum, etc.) that owns the text carrier digitizes it and makes it publicly accessible. Digitization follows established standards (e.g. [ISO standards](http://ikeep.com/ISO_14721){:target="\_blank"}) and maintains consistent quality. After the digitization process, the digitized copy is archived in a database by the memory institution for the long term.

Such public databases are usually operated by a network of memory institutions, e.g. [Patrinum](https://patrinum.ch/?ln=fr){:target="\_blank"} in the canton of Vaud or [e-manuscripta](https://www.e-manuscripta.ch){:target="\_blank"} in German-speaking Switzerland. There, the image data is made accessible with the [IIIF standard](https://www.digitale-edition.at/o:konde.123){:target="\_blank"}. This means that each document receives a IIIF-Manifest (describing the digitized text witnesses within) and can be retrieved via standardized interfaces.

!!! note "Experience from the Showcase Edition"

    In the constitution of texts for the Gaston Paris' exemplary letter edition, it was possible to draw on many years of research experience and comprehensive overview of the corpus. For a previous project, all of Gaston Paris' letters were digitized by the French National Library and made available online. Thus, we were able to quickly download [the relevant digital copies from their Gallica database](https://gallica.bnf.fr/ark:/12148/btv1b525187862){:target="\_blank"} for further processing.

    Due to download restrictions in Gallica, the images could not be accessed via the corresponding IIIF. Given the small scale of the project, this was not an issue. However, for larger volumes of images that need to be accessed via IIIF, we recommend contacting the database administration.

    To ensure remote access to the image data for all project members and facilitate the assignment of pages to Transkribus and the TEI Publisher, we created a [GitLab page for the image metadata](https://gitlab.uzh.ch/digital-editions/proto4diged/image-metadata){:target="\_blank"}.

The key advantage of this approach is that the long-term storage of the image data is not dependent on a time-limited project. This follows the **modular logic** of organizing the operation and preservation of the various DSE components independently (see [_project goals and resources_](../1_Planung/01_Projektziele_und_-ressourcen.en.md)).

**2.2 Digitization by a Memory Institution, Access Provided by the Project**

If the memory institution does not make the digitized material available in its own database - whether due to the absence of such a database, the selection being too small or too specialized, or the text carrier not being part of its own holdings - it is also possible to use a **IIIF server from another institution**. University libraries now often provide projects with storage space on such servers for a nominal fee. This additional financial cost - like all other server costs - must be secured for the duration of the project and beyond. In this case, the image data is not independently accessible via a database but can still be retrieved online using a dedicated URI.

**2.3 Digitization and Preservation by the Project**

A **project-led digitization** should be considered if access to a digitization service is difficult (e.g. if the holdings are stored in archives without a digitization department and transport to another institution is either not possible or impractical). Project-led digitization can also be considered if the project manages the text carriers itself, has access to professional scanners, and can delegate digitization work to assistants or similar personnel. It is important that the work is planned and supervised by specialists and is not carried out at the expense of research or editing time for academic staff (e.g. doctoral students or postdocs).
