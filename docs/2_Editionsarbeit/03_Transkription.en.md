# 2.2 Transcritpion, ATR and Annotation

## What does digital transcribing mean?

Transcription in non-digital editions was carried out according to transcription rules that had to be followed by assistant researchers or external transcription services. In contrast, the transcription process in DSE is characterised by more individual steps and decisions for the further course of the project. In particular, as described below, these are the choice of

1. the tool and the data formats;
2. the degree of automation;
3. the workflows in the actual transcription process (creating your own text recognition model; correction steps; possible initial annotations).

Finally, this handbook chapter will discuss the limitations of the standard transcription solutions available.

#### Transcription guidelines

As in print editions, consistent **transcription guidelines** must also be followed for DSE, especially with regard to **transcription scope** and **diplomatic transcription**, i.e. the degree of coverage of the transcription with the original in terms of linguistic and formal peculiarities: For manuscripts, the question must be answered as to which hands, (special) characters, textual interventions and revision stages are transcribed and how. In the case of prints, there is also the question of print-specific paratexts such as page numbers or bastard titles. The labelling of these formal textual aspects is also referred to as **text-critical annotation**; depending on the tool (see below), it can be carried out together with the transcription or only later together with the [_content annotation_](../2_Editionsarbeit/05_semantic_annotation.en.md).

!!! abstract "Showcase edition guidelines: Transcription and text-critical annotation"

    The showcase edition is intended as hypothetical preparatory work for a much larger edition of Gaston Paris's correspondence, comprising around 27,000 pages, which - if realised in later projects - will be aimed primarily at a **research audience**. Since the prototypical workflows developed are intended to fulfil scholarly standards of diplomatic editions on the one hand and must remain scalable in scope on the other, it concentrates on **the greatest possible textual fidelity with simultaneous simplicity of text-critical and content markup**.

    During the transcription process, the Showcase edition adhered to the following **text-critical principles**:

    **scope**

    - **All hands**, i.e. all different manuscripts, are transcribed.
        - Additions by **foreign hands**, i.e. which are not identified as the author's hand in the letter metadata, are identified as such by a text-critical annotation (see below, 3.5).=> Link example from the Showcase edition here.
        - Exception: Foreign hands are not transcribed if they concern additions of **archive signatures or archive pagination**. Archive signatures are contained in the metadata instead.

    - The question of **text-genetic sequences** (which hand can be assigned to which date) is not answered during the transcription by special characters or annotations, as Gaston Paris' letters are largely 'flat' in terms of text-genetics (i.e. they hardly show any traces of his own or other people's revisions). Where text-genetic contexts need to be presented, this is done in [_commentaries_](06_commenting.en.md).

    - Preprinted forms** (e.g. letterheads of hotels or private individuals) on the stationery are usually transcribed and also annotated text-critically as 'preprinted forms'. => Link example from the Showcase edition here.
        - Exception 1: Preprinted **form lines of postcards** ('Nom:', 'Prenom:', etc.) are not transcribed, as they are common to all postcards.
        - Exception 2: **Postcard cancellations or stamps** are not transcribed. The place and date information they contain can be recorded in the metadata if it differs from the date line of the letter. However, there are editions that have decided to label the postmarks in order to make them searchable, e.g. the [Gotthelf edition](=> add link here when published).

    **Diplomatic transcription**

    - Special characters used by Gaston Paris, particularly for scholarly reasons, or borrowed from foreign languages, are used tacitly and are not explicitly listed in a critical apparatus. Their understanding by the specialised audience is assumed.

    - Errors in the original manuscript are included without additional labelling. The error can be easily checked by comparing it with the manuscript displayed next to it.

    - Underlining, including double and triple underlining, and superscripts are transcribed as such.

    - Circling of words or letters is indicated by circling.

    - Conversion to blocking or bold type is omitted in order to preserve the often scientifically motivated emphasis of lemmata.

    - The French space before colons, semicolons and exclamation marks is used tacitly in the transcription. This last point deviates from a strict diplomatic transcription and is based on French printing conventions.

#### Reading version

A step that technically coincides with the text-critical and/or textual annotation, but which is not characterised by anything visible or substantive, is the creation of the **reading version**, which is placed alongside the more faithful diplomatic transcription (see also [_edition views_](../3_presentation/03_edition_views.en.md)). In order for the text to be normalised in a reading version, the words must be annotated with a correct or modernised word variant in the case of incorrect or outdated spellings - what is understood as incorrect or outdated must be [_documented_](../3_presentation/04_documentation.en.md) in detail.

!!! abstract "Showcase edition guidelines: Reading version"
    As the showcase edition of Gaston Paris' letters is primarily aimed at a scholarly audience, a reading version is not provided during the annotation process. However, this is also possible at a later stage, as the TEI/XML data can also be enriched at a later date using various tools.

#### Linking digitised material and transcription

DSE-specific transcription guidelines concern the **linking of digitised material and transcription** in the front end, i.e. the insertion of visual word or line correspondences between facsimile and text. Ideally, this is already prepared in the transcription step; all the tools mentioned below have simple forms of this link by enriching the XML file of the transcription with image coordinates. The line-by-line text-image link, which simplifies the autoptic comparison, e.g. by flashing the text line in the digital copy, has become the standard for DSE and is included below among the documented standard solutions.

!!! success "Best Practice"
    The [Briefedition Alfred Escher](https://www.briefedition.alfred-escher.ch/home.html){:target="\_blank"} is exemplary for the linking of digitised material and transcription for DSE using the TEI Publisher. .

    The Showcase edition is based on this form of line correspondence and utilises the existing [source code of the Alfred Escher letter edition](https://github.com/stazh/briefedition-escher){:target="\_blank"} was utilised.
    <figure markdown="span">

    ![screenshot Escher](image-3.png){ width="1000" }
    <figcaption>[Jung, Joseph (Hrsg.), Digitale Briefedition Alfred Escher, Relaunch January 2022, Zürich.](https://briefedition.alfred-escher.ch/briefe/B0056?view1=1){:target="\_blank"} Retrieved on 22.9.2024.</figure>


## 1. standard solutions for transcriptions

Once the text carriers have been selected and digitised, i.e. the [_Textkonstitution_](../2_Editionsarbeit/02_Textkonstitution.en.md) has been completed, the texts themselves must be made machine-readable. To do this, the image data of the digitised material, which is available in JPEG or TIFF format, for example, is converted into text data or transcribed. This can be done manually or automatically (see below), in both cases the same transcription tools and therefore the same XML standard data formats can now be used.

It is therefore advantageous to choose a scientific transcription tool for both manual and automated digital transcription and not a word processing programme such as Word. The latter does not use an open XML standard, does not allow transcription and digitised material to be linked by coordinates in XML or requires further data conversions.

Below we present the most common scientific transcription tools (a list of other tools can be found [here](https://www.adfontes.uzh.ch/ressourcen/quellen-erschliessen/digitale-transkriptionstools){:target="\_blank"} ):

- [Transkribus](https://app.transkribus.org/){:target="\_blank"} : The **most widely used transcription tool** as of 2024 is distributed by the international co-operative [READ-COOP](https://readcoop.org/de), which is owned by various academic institutions. It has extensive customer support and a large user community. Therefore, the tool can also offer the most AI models (developed by individual projects and provided by Transkribus) for text recognition. With the most advanced general AI model "The Text Titan 1", it is superior to all other transcription tools known to us as of summer 2024, at least as far as widespread manuscript types are concerned. However, Transkribus can only be used to a limited extent without paying for subscription offers.
- [eScriptorium](https://escriptorium.inria.fr/){:target="\_blank"} The code for this Transkribus alternative is provided free of charge by the Université PSL in Paris. It can be installed locally, but requires an **own server infrastructure** or institutional access to an eScriptorium server, as currently operated by various universities (e.g. the eScriptorium instance [fondue](https://fondue.unige.ch/){:target="\_blank"} of the University of Geneva can be used at most Swiss universities). The number of AI models available is currently growing rapidly.
- [OCR4all](https://www.ocr4all.org/){:target="\_blank"} : Like eScriptorium, the free transcription tool from the University of Würzburg requires installation on a local device or a dedicated server. It is currently less institutionally established than Transkribus and eScriptorium. A special feature of OCR4all is the automation not only of the text transcription step, but of entire workflows from uploading to saving in the desired format.
- [Transcribo](https://tcdh.uni-trier.de/de/projekt/transcribo){:target="\_blank"}  is a service offered by the Trier Centre for Digital Humanities at Trier University and part of its FuD research platform (comparable to [Textgrid](https://textgrid.de){:target="\_blank"} a German research network project). In contrast to the above tools, it allows transcription at word level instead of only at line level, i.e. each transcribed word refers to the word in the digitised text by means of coordinates. This allows greater accuracy to be achieved, but makes the process of manual transcription more complex. One DSE that uses this tool is the [Johann Caspar Lavater Online Briefedition](https://www.jclavater-briefwechsel.ch/home){:target="\_blank"} .

The Transkribus tool requires the least (project-specific) technical support, which is why we will focus on its workflows below. However, many work steps, such as training a model, can also be transferred to other tools.

As mentioned, the tools are also similar in terms of **data standards**: The transcription data can usually be output in an [XML format](https://www.digitale-edition.at/o:konde.215), e.g. in [PAGE-XML](https://www.digitale-edition.at/o:konde.154) or in [ALTO-XML](https://altoxml.github.io/). These are only preliminary stages for the DSE data standard [TEI/XML](https://www.digitale-edition.at/o:konde.79), in which the edition is ultimately made readable. A [_data conversion_](04_converting.en.md) must therefore take place between the workflow step of transcription in XML (including annotation, which is already possible here) and the more extensive [_content annotation_](05_semantic_annotation.en.md) and [_commenting_](06_commenting.en.md) in TEI-XML.

## 2 Automated or manual transcription?

There are cases in which manual transcriptions are still recommended. This applies in particular to editions of manuscripts: the more difficult the hand is to decipher and the smaller the quantity of manuscripts, the less worthwhile it is to use ATR. There are very capable general text recognition models such as "The Text Titan 1", especially for transcriptions, which recognise both prints and manuscripts - even in the same document. However, these are often not sufficient for **difficult hands**, which is why a hand-specific ATR model must be trained (see below). To train this model, a text volume of at least 75, in difficult cases even 200-300 training pages (so-called 'ground truth' = a corpus of prepared, correct transcriptions) is required until the ATR process (including training and subsequent corrections) no longer exceeds the manual effort. Only the transcription of a multiple of the required training pages justifies the use of a specific ATR model in these cases.

The decision in favour of automation therefore depends on a cost-benefit calculation: The aim of automatic text recognition is to minimise the correction effort, but in any case to keep it below the effort of manual transcription.
This is usually achieved by gradually expanding the training data with corrected transcriptions and training new text recognition models for manual transcription.
new text recognition models for the next data set.

## 3 Standard steps in the ATR process

If the decision in favour of ATR has been made, it is necessary to test whether an already available ATR model shows satisfactory results or whether a separate model should be trained. The standard transcription models maintained by Transkribus are constantly improving and it makes sense to carry out a test run with these models (if you are not aiming for your own model, you can continue with step 3.3).


### 3.1 Training an ATR model

As mentioned above, Transkribus recommends at least 75 pages of ground truth as a training set for your own transcription models. These can be existing transcriptions that are imported into Transkribus or pages that have been transcribed with the standard models and then corrected.

In the past, the **"text2image "** function was available for preparing existing transcriptions in Transkribus, which assigned existing transcriptions, e.g. from old print editions, to the digital copy line by line. At present, the line correspondences have to be created manually for training purposes. Such manual insertion of transcriptions into the training data only makes sense if it is not possible to use the standard models and make corrections. However, Transkribus has announced the reintroduction of "text2image" at the end of 2024.

!!! note "Experience from the showcase edition"
    For Gaston Paris' handwriting, the standard model "The Text Titan I" proved to be suitable for producing a ground truth with the help of corrections, which in turn allowed the training of a custom model (see next information box). This is an AI model that, similar to ChatGPT, is based on Transformer technology and is superior to conventional general ATR models that use older AI technologies. It is not yet possible to train Transformer models yourself on any transcription tool, but self-created ATR models can still compete with Tansformer models by training them with project-specific ground truth.

### 3.2 Repeated training, re-training

It is generally advisable to create **more than one specific model with the same ground truth**. Although the data basis does not change, the AI uses it to create a different model in each training session, which can differ greatly from the previous one in terms of the quality of text recognition. As a rule of thumb, at least four separate training runs should be carried out with a ground truth in order to minimise the randomness of the AI training. For example, the first training may already produce a good result, while the second is significantly worse, the third is the best and the fourth is worse again.

Re-training with a larger ground truth** differs from repeated training with the same ground truth. When should better models be trained with new data? This question can also only be answered on a project-specific basis. Factors are

- Quality improvement;
- Correction effort;
- Available time of the project members;
- Time needed for training.

!!! note "Experience from the Showcase Edition"
With the help of ever larger ground truth collections (manually corrected transcriptions that we created with "The Text Titan I"), several series of re-trainings were made; the second model of the second series surpassed "The Text Titan I" in certain recognition performances, namely in rather exceptional idiosyncrasies of Gaston Paris' handwriting. However, the general model continued to 'beat' its own in the recognition of numbers and different languages.

### 3.3 Layout analysis

In layout analysis, an algorithm recognises **the arrangement of the lines** before the actual text recognition is performed; it is therefore not an optional step like the annotation of text or text regions (see below, 3.5). While older versions of Transkribus required layout analysis as a separate, preliminary step before ATR, this multi-stage process is now optional and text recognition can be started directly (using a specific or a general model). Only in the case of poor transcription results, in which lines have been partially or completely omitted, is it advisable to try out different models and configurations for layout analysis.

### 3.4 Correcting the layout analysis and transcription

During the correction process, it is advisable to first check the lines, especially if lines have been recognised as fragmented or missing. Very poor results of the layout analysis justify tests with different layout analysis models (see above).

If this does not bring any improvement, the **lines can also be improved manually or pulled out completely by hand**. Layout corrections such as lengthening a line improve a new ATR run and the visual correspondence between transcription and digitised text in the frontend (see our [_Tips_](../Themen/transkribus.en.md)). However, a precise revision of the lines may represent an unjustifiable additional expense, as the comparison is also possible without this overlay thanks to the visual overlay of the line correspondence.

Errors in the transcription can simply be corrected in the lines. Incorrect line regions can also be corrected in this step. However, it should be noted that when using the optional word segmentation, the individual words cannot be corrected - for this step, post-processing in Transcribo (https://tcdh.uni-trier.de/de/projekt/transcribo){:target="\_blank"}  is an option.

### 3.5 Annotations in the transcription tool

The last, already optional step in Transkribus and similar transcription tools is the **annotation ('tagging') first of text regions and finally of the text itself**. The first step, the determination of the text region, is optional, but only with regard to the question of when, not whether, it takes place. The **annotation at region level** is a standard feature of a DSE, as it fundamentally structures the text, e.g. into paragraphs, postscripts, verses, etc.

The more detailed annotation of word sequences or words is also part of the standard, but its level of detail is less standardised and, depending on the edition guidelines, may only include a minimal set. A basic distinction is made between **two forms of annotation at word level**:

- **Text-critical annotations** characterise visible features of the typeface, such as underlining.
- Content annotations** characterise semantic properties of the text, such as the definition of a geographical location. This form of annotation will be discussed in more detail [_later_](05_semantic_annotation.en.md).

From a technical point of view, these steps no longer constitute a transcription of the text, but could also take place later in the TEI/XML. However, there are reasons why the annotation of regions and text-critical aspects - i.e. features recognisable in the typeface - is already carried out during the transcription (or its correction): The labelling of different hands, underlining, titles, paragraphs, etc. is already closely linked to it. If the digital copy and the finished or emerging transcribed text have to be compared with each other exactly, it makes sense to record not only the correct (e.g. diplomatic) character sequence but also the **visible peculiarities of the text**.

Transkribus distinguishes between 'structural tags' and 'textual tags', which corresponds to the distinction drawn above between annotation at region level and annotation at word level.

![alt text](image.png){align=left width="250" } With **'Structural Tags'**, self-definable text regions and line regions automatically generated by the layout analysis ('base lines' and associated 'line polygons') can be marked up directly on the digital copy, i.e. on the left-hand side of the user interface. Even if these tags appear on the digital copy for the sake of simplicity, they are saved in the same XML file as the transcription.

![alt text](image-2.png){align=right width="250" }**'Textual Tags'** allow tagging at the word level of the transcription and are therefore attached to the transcription text on the right-hand side of the user interface. In addition to formal aspects (underlining, foreign hands), 'textual tags' can also include content-related aspects (tagging of place names or keywords). However, we recommend that the more complex content annotation is only carried out in TEI-XML in order to minimise the conversion effort (see below). Transkribus is also not (yet) capable of automatically linking content annotations to external resources such as standardisation data. Even if this should change in the future, as is apparently planned, caution is advised due to the conversion effort involved.

!!! warning "challenge"
    As already mentioned, transcription tools offer markup in PAGE-XML or ALTO-XML, which must be taken into account when converting to TEI-XML.
    It is therefore advisable to orientate yourself **in the markup in the transcription tool to the nomenclature of the TEI/XML you are aiming for**. In this way, TEI syntax-compliant elements are created during conversion to TEI/XML instead of freely invented expressions or - if not marked up - anonymous blocks (`<ab>`). The most important elements are recognised by scripts such as Page2TEI by default and converted into the corresponding elements. This represents an increase in complexity that requires close technical support for the project.

The advantage of annotations in transcription tools is that the most important formal aspects can already be clarified in the initial, superficial examination of the text. In the next steps after conversion, content annotation and commenting - which are described in the following chapters primarily using the TEI Publisher - the employees can then deal more intensively with the semantic aspects.
Projects should consider as early as possible whether and how thoroughly they should work with the transcription tools' tags, which are easy to use but demanding in the conversion process.

!!! note "Experience from the showcase edition"
    We have decided to use 'Structural' and 'Textual' tags in Transkribus only for text-critical aspects (see showcase edition guidelines above). In this labelling of Gaston Paris's letters, we adhere to the element names that the [German text archive](https://www.deutschestextarchiv.de/){:target="\_blank"} suggests as the [basic format for labelling letters](https://deutschestextarchiv.de/doku/basisformat/brief.html){:target="\_blank"} suggests. For this purpose, we have created our own tags in Transkribus and used them in the labelling of the text regions on the digital copy: The letterhead, for example, is defined as the text region 'opener', in this text region we mark up the line with date and, if applicable, place as 'dateline' and the greeting ("Mon cher ami") as 'salute'. The text body itself is divided into different paragraphs.

    ![Tagging in Transkribus](image-1.png)

## 4. limitations

### 4.1 The ideal transcription tool?

There is currently no single solution for transcription. The tools listed above mainly require **different amounts of support and technical knowledge**, but have similar functionalities. It seems advisable to us to base the choice of tool more on existing institutional know-how and technical resources than on the capabilities of the tool (especially because these capabilities are similar in the tools portrayed above). If the institutional know-how is very limited and the financial situation allows a Transkribus subscription, we would argue in favour of such a subscription.

### 4.2 ATR as a solution?

The high hopes placed in scientific applications of AI also apply to ATR models, which are sometimes based on the same technology as large language models (e.g. ChatGPT). Although the advances in ATR are currently very great, they are not yet great enough, especially with regard to older and/or difficult handwriting, for their use in every DSE project to make sense.
Even when using the best available ATR models, the correction effort can exceed a manual transcription from the outset. Training your own models is time-consuming and does not always lead to better results. It is therefore imperative that projects plan a **test phase** in which they evaluate the options before large ground truth collections are created and trained.

### 4.3 Annotating in transcription tools?

The question of how much should be annotated in PAGE-XML or ALTO-XML also depends on the available technical support. We are aware of projects whose workflow provided for extensive annotations in Transkribus, not only in terms of textual criticism but also in terms of content, and had to put up with major delays and adjustments to the workflow due to conversion difficulties. It must therefore be clear from the start of the project **where which annotations should take place** in order to adapt the complexity of the data conversion to the project resources.
The Showcase edition has extended the annotation editor interface so that text-critical annotations would also be possible entirely in the TEI Publisher. The procedure is the same as we have described for [_content annotation_](05_semantic_annotation.en.md).
