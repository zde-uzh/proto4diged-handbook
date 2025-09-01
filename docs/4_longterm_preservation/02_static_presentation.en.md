# 4.1 Static Presentation

**Why Static Presentations for DSE?**

As described in the introduction to long-term preservation, static forms of presentation currently (as of 2024) appear to be a promising solution for ensuring the **long-term preservation of a DSE, including most of its user functions**. A static DSE presentation primarily consists of pre-generated HTML or JSON files. This eliminates the need to maintain a database, which is necessary for dynamic presentations. Domain-specific knowledge of XML databases and their long-term maintenance is thus no longer required. Static websites can be handed over by technical DH and DSE specialists to a general IT service within a research or memory institution, for example, one that is also responsible for maintaining other simple websites.

???+ question "Static vs. dynamic web presentations"

    **Dynamic presentation with database**

    ![alt text](Web_server_serving_static_and_dynamic_content.png)

    CC BY-SA 4.0: Ade56facc [https://commons.wikimedia.org/wiki/File:Web_server_serving_static_and_dynamic_content.png](https://commons.wikimedia.org/wiki/File:Web_server_serving_static_and_dynamic_content.png){:target="\_blank"}

    **Static presentation without database**

    ![alt text](Web_server_serving_static_content.png)

    CC BY-SA 4.0: Ade56facc [https://commons.wikimedia.org/wiki/File:Web_server_serving_static_content.png](https://commons.wikimedia.org/wiki/File:Web_server_serving_static_content.png){:target="\_blank"}

### Differentiation from the Static User Experience

Irrespective of the above distinction between dynamic and static presentations based on their implementation on the server, the terms static and dynamic are also used in reference to the user experience (i.e., the ways in which users can interact with the content of websites).
However, this is a result of the frontend implementation, i.e., the format within the pre-generated files. This is not what is meant in the following discussion.

## Static Presentation with TEI Publisher 10

In version 9 of the TEI Publisher, publication of the DSE is only intended as a dynamic presentation. For this, [a dynamic app is generated](https://teipublisher.com/exist/apps/tei-publisher/documentation/create-app){:target="\_blank"} in the TEI Publisher, which then requires ongoing maintenance. In version 10 of the Publisher, a **static generator** will become a central feature of the publication options. Additionally, an **App Manager** will automate the process of creating a custom app for an edition.
Ideally, this will enable the generation and testing of various versions of static presentations throughout the course of the project.

There are also plans for intermediate forms that preserve certain dynamic functions of the presentation. If these functions can no longer be maintained, the rest of the DSE should remain functional.

## Other Static Presentation Tools

Various tools and scripts already exist that allow the conversion of dynamic websites into static ones. However, using these tools typically requires more technical expertise than the static generator planned for TEI Publisher.

-   [Eleventy](https://www.11ty.dev/){:target="\_blank"} has already been used with older versions of TEI Publisher. In 2022, e-editiones developed its own [plugin from Eleventy for the TEI Publisher](https://github.com/eeditiones/tei-publisher-eleventy){:target="\_blank"} and provided [detailed documentation](https://www.e-editiones.org/posts/community-event-going-static/){:target="\_blank"} on its use.

-   The [Austrian Centre for Digital Humanities and Cultural Heritage (ACDH-CH)](https://www.oeaw.ac.at/acdh/acdh-ch-home){:target="\_blank"} has developed a static website generator for DSE called [DSE-Static-Cookiecutter](https://github.com/acdh-oeaw/dse-static-cookiecutter?tab=readme-ov-file){:target="\_blank"}.This tool has been, or will be, used for various editions related to Arthur Schnitzler, such as his [Diary](https://schnitzler-tagebuch.acdh.oeaw.ac.at){:target="\_blank"}, his [Letters](https://schnitzler-briefe.acdh.oeaw.ac.at/){:target="\_blank"}, and his [correspondence with Hermann Bahr](https://schnitzler-bahr.acdh.oeaw.ac.at/){:target="\_blank"}.
    One of the advantages of this tool is that it can directly publish TEI/XML source data as a static website via a GitHub repository. This means that [_archiving the data_](../4_longterm_preservation/03_archiving_data.en.md){:target="\_blank"} and its presentation are closely linked - any update to the dataset automatically generates a new version of the presentation.

    However, it is important to note that **GitHub** does **not** meet the criteria for a **FAIR repository**. It is a privately operated platform with no guarantees for open licensing or metadata curation, does not assign PIDs (Persistent Identifiers), and has notable limitations regarding data protection. The University Library of Zurich provides an overview of FAIR data archiving and repository standards[here](https://www.ub.uzh.ch/de/wissenschaftlich-arbeiten/mit-daten-arbeiten/daten-ablegen-und-teilen.html){:target="\_blank"}.

-   One of the most widely used tools for generating static websites is [Jekyll](https://jekyllrb.com/){:target="\_blank"}, the tool behind GitHub Pages. However, we are not aware of any DSE projects that use Jekyll, as it does not natively convert XML data into HTML without additional intermediate steps or tools. Instead, Jekyll is primarily designed for Markdown-based content.

## General Limitations

For complex editions that rely on a **large database** and require **constant updates**, generating a static presentation is often impractical. While static websites load faster, they only display a pre-generated snapshot, which can quickly become outdated as the project evolves.

Another key limitation of static presentations is the potential loss of **search functions** and **visualization features, such as timelines or geographical maps**. For example, the static presentation generated using the TEI Publisher Eleventy plugin is restricted to basic searches, meaning that more advanced capabilities like [faceted search](https://en.wikipedia.org/wiki/Faceted_search), which databases typically provide, are either limited or require more sophisticated indexing. Similarly, visualization tools that depend on external resources can still be integrated into a static presentation, but their functionality will depend on the availability and stability of those external resources.

## Limitations of Data Formats for Static Presentation

The following section introduces HTML and JSON as the two primary data formats into which TEI/XML data must be converted for static presentations. This section is primarily intended for technically trained editors.

### HTML-Based Presentations

The **most drastic approach** is converting edition data into HTML files, making them as static as a printed book. In this format, content and presentation are no longer separated. The advantage of HTML is its longevity - data remains accessible in a durable format and can be viewed offline in a web browser with minimal effort.

However, this approach has significant drawbacks. Different views of the same content must be converted separately, each receiving its own distinct file path. As a result, **linking** between various sections depends directly on the conversion process and must be carefully managed during updates.

Additionally, **search functionality is not available** in purely HTML-based presentations without a supporting database. To enable search, one must rely on external providers like search engines or adopt a hybrid approach, integrating features such as search functionality using JavaScript.

HTML-based editions must be designed from the outset with this format in mind. XSLT transformations can be used as a tool for conversion.

==->@How sustainable is an XSLT conversion on the fly in the browser?

### JSON-Based Presentations

A less extreme approach is using JSON files that contain data equivalent to what would be retrieved from a database interface, with HTML serving only as a format for individual properties.
With this method, converting an existing dynamic presentation into a static one remains **feasible even at a later stage**, while still preserving the dynamic user experience.

However, this approach comes with some drawbacks. It **relies heavily on rapidly evolving JavaScript libraries** (especially for full-text search), and the edition can only be accessed locally via HTTP.

**Search functions** can be implemented using libraries like [FlexSearch](https://github.com/nextapps-de/flexsearch){:target="\_blank"}, allowing searches to be performed directly in the browser. However, the format of the search index data depends on the specific library used, meaning that switching libraries would require a complete reimplementation. Additionally, loading a search index for large datasets increases data traffic.


