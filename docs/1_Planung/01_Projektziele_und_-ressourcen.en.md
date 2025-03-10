# 1.1 Definition of the Project Goals

Unlike humanities research, which is at least ideally open-ended, work on DSE must **start with the end product in mind**. Planning must be guided by a model of the completed edition and its intended uses, working backward from the desired outcome to determine the necessary workflow steps, while continuously refining this outcome throughout the planning process.

In the following, we outline questions and challenges that should be clarified during the planning phase as part of a **requirement check**. The following chapters of this handbook help refine the provisional answers during the planning phase.

### 1. Starting Point: Project Framework and Resources

Before starting the detailed planning of the end product, the following factors should be evaluated:

-   Nature and quantity of the data to be edited (see [_constituting texts_](../2_Editionsarbeit/02_Textkonstitution.en.md))
-   Team size and skills
-   Project duration

The evaluation of these factors heavily depends on the institutional and financial situation, particularly the availability of funding. In the case of Switzerland, for example, as of summer 2024, public funding for larger DSE is only possible as part of a 4-year [project application to the Swiss National Science Foundation](https://www.snf.ch/de/WAvYcY7awAUGolST/foerderung/projekte/projekte-in-allen-disziplinen){:target="\_blank"}. This example is meant for illustration only, of course, as funding opportunities can change rapidly and require thorough investigation.

### 2. Coordination of the Technical Components

One technical principle of DSE is the **modular logic** of organizing the operation and backup of the various DSE components independently of each other. In particular, image data, the edition database (TEI/XML data), and the edition front end should be kept separate so that they can be transferred to other institutions, replaced, or supplemented with new technical solutions as needed.

Before tools and platforms are defined, DSE projects should consider the coordination of the technical components.

-   Is there a **technical lead** who is familiar with all components?

    -   If not, how is the coordination handled?

-   Are all available **technical components really necessary**?
    -   Small projects, for example, can do without metadata databases and curate their metadata in Excel or CSV files.

### 3. Forms of Publication

-   Does the final product need to be a digital publication with an interface that is as easy to maintain as possible (see our chapter about [_static presentation_](../4_longterm_preservation/02_static_presentation.en.md))?
-   Are there plans for a printed edition based on a [_reading version_](../3_presentation/03_edition_views.en.md/#reading-versions)?
-   Is the frontend an intermediate stage that will be replaced by other forms of publication after a certain period (e.g. on a larger platform)?

### 4. Different Forms of Data Usage

How should the **data** of the edition be used?

-   For qualitative analysis (e.g. historical source evaluation, philological text-genetic or hermeneutic methods), it is worth focusing on the [_digital presentation_](../3_presentation/01_introduction_presentation.en.md) and designing the texts on the _human-readable_ interface, i.e. preparing them (also) for human use. In essence, the main goal should be achieving the best possible [_accessibility_](../Themen/accessibility.en.md).
-   For quantitative analysis (e.g. corpus linguistic analyses, philological distant readings, statistical questions), [_long-term preservation in databases_](../4_longterm_preservation/03_archiving_data.en.md) a key consideration. It makes the data (also) _machine-readable_ via technical interfaces, so-called APIs, i.e. the data can be read automatically by programs and tools.

Of course, the two options are not mutually exclusive. A project can enable both qualitative and quantitative analysis scenarios. In many cases it is even advisable to enable both.

### 5. When is Automation Worthwhile?

Repetitive tasks are ideal candidates for **automation**, but not every repetitive task is worth automating. For example, one should consider what takes longer: adapting or rewriting a Python script, or the repetitive work of a research assistant? The project must recruit the necessary technical expertise.
