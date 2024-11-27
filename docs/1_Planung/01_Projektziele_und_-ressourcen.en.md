# 1.1 Definition of the project goals

Unlike humanities research, which is at least ideally open-ended, DSE must be conceived **from the point of view of the end product**. Planning must be based on a model of the finished edition and its intended use, and the necessary workflow steps must be traced back from the desired result - admittedly not without continuously adapting this result in the planning process.

In the following, we outline questions and challenges that a project should clarify for itself in the planning phase in the sense of a **requirement check**. The provisional answers should be concretised in the planning phase with the help of this handbook.

### 1. Initial situation: project framework and resources

Before detailed planning of the end product can begin, the following factors should be evaluated:

- Nature and quantity of the media to be edited (see [_constituting texts_](../2_Editionsarbeit/02_Textkonstitution.en.md))
- Team size and skills

- Project duration

The extent to which these factors can be adapted depends on the institutional and financial starting position, in particular possible funding. In the case of Switzerland, for example, as of summer 2024, public funding for larger DSEs is only possible as part of a 4-year [project application to the Swiss National Science Foundation](https://www.snf.ch/de/WAvYcY7awAUGolST/foerderung/projekte/projekte-in-allen-disziplinen){:target="\_blank"} is possible.

### 2. Interaction of the technical components

A technical principle of DSE is the **modular logic** of organising the operation and backup of the various DSE components independently of each other. In particular, image data, the edition database (TEI/XML data) and the edition front end should be kept separate from each other so that they can be transferred to other institutions or replaced or supplemented with new technical solutions as required.

Before tools and platforms are defined, DSE projects should think about the interaction of the technical components.

- Is there a **technical lead** who is familiar with all components?

    - If not, how is the interaction coordinated?

- Are all available **technical components really needed**?
    - Small projects can, for example, dispense with metadata databases and curate their metadata in Excel or CSV files.

### 3. Forms of publication

- Must a digital publication of the interface that is as easy to maintain as possible be available at the end (see our chapter about [_static presentation_](../4_longterm_preservation/02_static_presentation.en.md))?
- Are physical prints planned that are based on a [_reading version_](../3_presentation/03_edition_views.en.md/#reading-versions)?
- Is the frontend an intermediate stage that will be replaced by other forms of publication after a certain period of time (e.g. on a larger platform)?

### 4. Different forms of data utilisation

- How should the **data** of the edition be used?

    - For qualitative analysis (e.g. historical source evaluation, philological text-genetic or hermeneutic methods)? Then it is probably worth focussing on a [_digital presentation_](../3_presentation/01_introduction_presentation.en.md).
    - For quantitative analysis (e.g. corpus linguistic analyses, philological distant readings, statistical questions)? Then the [_long-term preservation in databases_](../4_longterm_preservation/03_archiving_data.en.md) is in the foreground.

### 5. Where is automation worthwhile for the project?

Repetitive work is predestined for **automation**, but not all repetitive work is worth automating (specifically: what takes longer: adapting/rewriting a python script or the repetitive work of a research assistant?) Appropriate technical knowledge must be recruited for the project.
