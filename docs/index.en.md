# Manual Proto4DigEd: Prototypical Workflows for Digital Scholarly Editions (DSE)

## 1. The manual

### Scope

The handbook supports researchers and projects from the humanities in the creation of digital scientific editions (DSE) throughout their entire duration, i.e. from the planning phase to long-term preservation. Its focus on text editions is based on our experience in the Proto4DigEd project.

!!! note "Creation of the showcase edition"
    [Proto4DigEd](https://www.zde.uzh.ch/de/projects/proto4diged.html){:target="\_blank"} is an Open Research Data project, supported by swissuniversities, 2023-2024, under the direction of [Prof. Dr Ursula Bähler](https://www.rose.uzh.ch/de/seminar/personen/baehler.html){:target="\_blank"}. Representatives from the fields of literature and history, digital humanities and librarianship tested and evaluated editing workflows using a partial corpus of the correspondence of the French philologist Gaston Paris. The DSE standard tools **Transkribus** (for text recognition and transcription) and **TEI-Publisher** (for annotation, commenting and publication) were used for the edition.

    Our approach in the resulting **Showcase Edition** is referenced at relevant points in the handbook in information boxes (such as this one). On the one hand, these contain specific editing guidelines such as the [_Transcription guidelines_](../2_Editionsarbeit/03_Transkription.en.md) applied, thus providing an insight into how a project documents its approach (which we reflected on a methodological level in the [_Dokumentations-Kapitel_](../3_presentation\04_documentation.en.md)). On the other hand, there are more general "Experiences from the showcase edition" in information boxes, in which we point out challenges in the workflow - for example, that [_Setting up the annotation editor in TEI Publisher_](../2_Editionsarbeit/05_semantic_annotation.md/) was a complex team process. Editorial decisions and forms of presentation are also symbolised by links in the edition. However, it is important to note that although these are exemplary solutions, they are by no means unique.

However, the handbook does not only document tools evaluated in Proto4DigEd; its basic edition science considerations for planning workflows can also be applied to editions of non-textual or multimedia media with certain restrictions. In order to be accessible to researchers who have previously worked on printed editions, it uses tried and tested **editorial terms** (text constitution, transcription, diplomatic transcription, etc.), but reflects their transfer to digital, which can lead to shifts in meaning or extensions.

The handbook does not claim to cover all facets of digital editing; it supplements resources that are already available or will soon be available that focus on individual workflow steps, above all the [KONDE Weißbuch](https://www.digitale-edition.at){:target="\_blank"} as a standard reference work. This provides basic insights into various topics, but does not offer any procedural considerations for planning workflows. This manual refers extensively to the KONDE White Paper to avoid duplication.
More specific manuals include [PATT](https://www.hist.uzh.ch/de/fachbereiche/mittelalter/lehrstuehle/teuscher/forschung/projekte/PATT.html){:target="\_blank"} for automatic text recognition for historians, [DigEdTnT](https://digedtnt.github.io/about/){:target="\_blank"} for the transition between tools, or the [Manual for the creation of non-discriminatory metadata for historical sources and research data](https://maehr.github.io/diskriminierungsfreie-metadaten/){:target="\_blank"}.

### Goal: Recognising and weighing up options

The prototypical, i.e. exemplary, steps in the creation of DSE documented here are intended to serve as a guide. They provide an overview of tried and tested workflows of available tools (see below for these terms), which require different degrees of skills and resources.
 
The manual therefore always reflects a **multitude of possibilities** and helps DSE projects to weigh them up. The aim of the documentation is not to provide _the_ perfect path or workflow for every project. Instead, it provides tips for planning and implementing DSE that are appropriate to the project framework. These factors have a fundamental impact on the [_planning_](1_planning/01_project_objectives_and_resources.en.md). If necessary, reference is also made to (previously) unfeasible paths. Sharing knowledge about workflows supports the implementation of the [FAIR Data Principles](https://www.go-fair.org/fair-principles/){:target="\_blank"}, i.e. it enables the findability, accessibility, interoperability and reuse of data - in this case data relating to digital editing methods that are made accessible by both external and self-generated resources.

## 2. Workflows

We understand a **workflow** as a sequence of consecutive work steps, the completion or completeness of which is based on an editorial decision. The completion of [_Text constitution_](2_Editionsarbeit/02_Text constitution.md) is an editorial decision - based on the overall planning - that allows us to proceed to [_Transcription_](2_Editionsarbeit/03_Transcription.en.md) of the corpus. There is a separate entry for each of these work steps in the handbook, whereby the sub-chapters on "editing work" are most closely organised as a workflow process.

Workflow steps can be divided per se between different employees or teams, in contrast to sub-steps, which often prohibit this (partly because their finalisation depends less on editorial than on technical considerations). However, the **division of labour** within the workflow always requires precise planning and coordination; it does not always make sense. The manual refers to particularly closely interlinked work steps.

### Complexity

In recent years, workflows have increasingly moved into the **focus of the digital humanities** and in particular the discussion of DSE (cf. e.g. [DARIAH Annual Event 2024: "Workflows: Digital Methods for Reproducible Research Practices in the Arts and Humanities"](https://www.dariah.eu/2023/12/12/dariah-annual-event-2024-workflows-digital-methods-for-reproducible-research-practices-in-the-arts-and-humanities/){:target="\_blank"}). The background to this interest is, on the one hand, an **increase in complexity**: The number of ever more easily accessible tools and platforms for DSE is increasing. It is important to select from them for specific project requirements in order to integrate them into a workflow and harmonise them with one another.

### Standardisation

On the other hand, the increase in complexity of available tools and platforms is offset by the standardisation of (meta) data formats and standards, in particular the use of [_TEI/XML_](topics/tei.md){:target="\_blank"} for structuring and annotating machine-readable edition texts and linking the annotations to the metadata of [_Normdatenbanken_](Themen/authority.md). This standardisation of data and the associated standardisation of editing guidelines and functionalities of DSE leads to an increasing **demand for standardisation of workflows**. Where similar data/publications are to be compiled, similar workflows can also be used. This is also an aspect of the FAIR principles, the operationalisation of which is the subject of an [issue of the specialist journal RIDE]( https://ride.i-d-e.de/issues/issue-16/editorial/){:target="\_blank"}.

We are particularly interested in the _how_: How and when does it make sense to generate different, often self-created workflows? To what extent can tools and platforms be combined in best practices and in a standardised way? And what editorial and technical restrictions are associated with this standardisation, i.e. what **editorial scope for decision-making** is lost as a result? The manual is therefore intended less as a guide to the actual standardisation of workflows and more as an aid to determining the degree of standardisation of workflows and developing a project-specific best practice. For this reason, the individual workflow chapters, especially in the main chapter "Editing", are organised according to the following pattern:

1. explanation of the workflow step

2. description of the existing standards (and possible alternatives)

3. evaluation of the limitations of standard tools
    - We sometimes refer to 'haute couture' solutions, i.e. 'customised' functionalities for which no standardisation exists

## 3. Tools and platforms

This manual defines a **tool** for creating a DSE as any relevant technical tools and aids; in addition to desktop or web-based programmes, these can also be add-ons or code scripts that require different levels of prior technical knowledge to use. The manual provides information on how much prior knowledge is required in which cases. At its centre are the widely used tools [Transkribus](https://app.transkribus.org/){:target="\_blank"} and [TEI-Publisher](https://teipublisher.com/){:target="\_blank"}.

In addition to the category of tools, the category of **(publication) platforms** is central, as they ensure the accessibility of the DSE and its (meta)data. These include centrally managed databases (such as the [Swiss National Data and Service Centre for the Humanities DaSCH](https://www.dasch.swiss/){:target="\_blank"}), metadatabases (such as [Metagrid](https://metagrid.ch/){:target="\_blank"} or [Correspsearch](https://correspsearch.net)) and repositories for various types of data (not DSE-specific: [Zenodo](https://zenodo.org/), [Swissubase](https://www.swissubase.ch/en/), [GitHub/GitLab](https://github.com/){:target="\_blank"}; DSE-specific: repositories for transcription data such as [transcriptiones](https://transcriptiones.ch/){:target="\_blank"} or [htr-united](https://htr-united.github.io/){:target="\_blank"}). Like different tools, platforms also require different prior knowledge or training periods, but above all they are aimed at different audiences and fulfil different purposes. In contrast to tools, the choice of which often entails workflow decisions that are difficult to reverse, the use of several platforms for [_presentation_](3_presentation/01_introduction_presentation.en.md) and [_longterm preservation_](4_longterm_preservation/01_introduction_preservation.en.md) of the DSE and its data is expressly recommended.

### Obsolescence and innovation

What the manual is _not_ in technical terms: The documented steps are **not instructions** on how to use specific tools or platforms in detail. As development is currently progressing rapidly, a high level of detail would quickly lead to the documentation of outdated features. Just as the manuals on printed editing are still valid today in their editorial considerations, this manual is also linked to the hope of continuing to offer help after future technical innovations.

This already addresses a fundamental challenge of digital editorial work: on the one hand, it is dependent on the limitations and obsolescence of technical tools; on the other hand, innovative editorial possibilities arise from their further development. The balance between scientific necessity ("scientifically and editorially necessary") and innovative surplus ("nice to have") must therefore always be kept in mind when planning, especially when clarifying the [_project objectives_](1_Planung/01_Projektziele_und_-ressourcen.md).
