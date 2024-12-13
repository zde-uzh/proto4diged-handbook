# 4.1 Static Presentation

## Why static presentations from DSE?

As described in the introduction to long-term preservation, static forms of presentation currently (as of 2024) appear to be a promising solution to ensure **long-term preservation of a DSE including most of its user functions**. A static DSE presentation consists primarily of HTML or JSON files that have been pre-generated. This eliminates the need to maintain a database, which is necessary for dynamic presentations. Domain-specific knowledge of XML databases and their long-term maintenance is therefore no longer necessary. Static websites can be handed over by technical DH and DSE specialists to a **generalist IT service** of a research or memory institution, for example, which is also entrusted with the maintenance of other simple websites.

???+ question "Static vs. dynamic web presentations"

    **Dynamic presentation with database**

    ![alt text](Web_server_serving_static_and_dynamic_content.png)

    CC BY-SA 4.0: Ade56facc [https://commons.wikimedia.org/wiki/File:Web_server_serving_static_and_dynamic_content.png](https://commons.wikimedia.org/wiki/File:Web_server_serving_static_and_dynamic_content.png){:target="\_blank"}

    **Static presentation without database**

    ![alt text](Web_server_serving_static_content.png)

    CC BY-SA 4.0: Ade56facc [https://commons.wikimedia.org/wiki/File:Web_server_serving_static_content.png](https://commons.wikimedia.org/wiki/File:Web_server_serving_static_content.png){:target="\_blank"}

### Differentiation from the static user experience

Irrespective of the above division into dynamic and static presentations based on their implementation in the server, the terms _static_ and _dynamic_ are also used for the user experience (i.e. the ways in which the content of websites can be interacted with).
However, this is a consequence of the implementation of the front end, i.e. the format _in_ the pre-generated files. This is not what is meant below.

## Static presentation with the TEI Publisher 10

In version 9 of the TEI Publisher, publication of the DSE is only intended as a dynamic presentation. For this purpose, [a dynamic app is generated](https://teipublisher.com/exist/apps/tei-publisher/documentation/create-app){:target="\_blank"} in the TEI Publisher, which must then be maintained. For version 10 of the Publisher, a **static generator** is to become a central component of the publication options. There will also be an **App Manager** that automates the process of creating a custom app for an edition.
Ideally, this will make it possible to output and test different versions of static presentations during the course of the project.

Intermediate forms that retain certain dynamic functions of the presentation are also envisaged. If these functions can no longer be maintained, the rest of the DSE should remain functional.

## Other static presentation tools

Tools or scripts already exist today that allow the conversion of dynamic websites into static websites. However, their use requires more technical knowledge than the use of the static generator announced above in TEI Publisher promises.

-   Eleventy](https://www.11ty.dev/){:target="\_blank"} has already been used for older versions of the TEI Publisher. e-editiones has developed its own [plugin from Eleventy for the TEI Publisher](https://github.com/eeditiones/tei-publisher-eleventy){:target="\_blank"} in 2022 and [documented] its use in detail. and [documented](https://www.e-editiones.org/posts/community-event-going-static/){:target="\_blank"} its use in detail.

-   The [Austrian Centre for Digital Humanities and Cultural Heritage (ACDH-CH)](https://www.oeaw.ac.at/acdh/acdh-ch-home){:target="\_blank"} has developed the tool [DSE-Static-Cookiecutter](https://github.com/acdh-oeaw/dse-static-cookiecutter?tab=readme-ov-file){:target="\_blank"} a static website generator for DSE, which is or will be used for various editions on Arthur Schnitzler (Schnitzler's [Diary](https://schnitzler-tagebuch.acdh.oeaw.ac.at){:target="\_blank"}, his [Letters](https://schnitzler-briefe.acdh.oeaw.ac.at/){:target="\_blank"} and [Letters and materials from his correspondence with Hermann Bahr](https://schnitzler-bahr.acdh.oeaw.ac.at/){:target="\_blank"}).
    The advantage of this tool is that it can publish TEI/XML source data directly via a GitHub instance on a GitHub repository as a static website (the [_Archiving the data_](../4_longterm_preservation/03_archiving_data.en.md){:target="\_blank"} and its presentation are thus directly linked to each other and a new version of the data status automatically leads to a new version of the presentation).

    However, it should be noted that **Github** does **not** fulfil the requirements of an **FAIR repository**. It is operated by a private provider without specifications for open licences or curation of the metadata, no PIDs (Persistent Identifiers) are assigned and, above all, there are data protection limitations. The University Library of Zurich provides an overview of the criteria for FAIR data archiving and repositories [here](https://www.ub.uzh.ch/de/wissenschaftlich-arbeiten/mit-daten-arbeiten/daten-ablegen-und-teilen.html){:target="\_blank"}.

-   One of the most widely used tools for generating static websites is [Jekyll](https://jekyllrb.com/){:target="\_blank"}, the tool behind the output of GitHub pages. However, we are not yet aware of an application for DSE projects, especially as Jekyll cannot convert XML data into HTML without further intermediate steps or tools, but specialises in MarkDown data.

## General Limitations

For complex editions that rely on a **large database** and want to **constantly expand** it, generating a static presentation makes little sense. Although calling up a static website is faster, it only ever displays a pre-generated snapshot that quickly becomes outdated as the work in progress continues.

When converting to static presentations, it should also be noted that certain **search functions** and the **display of timeline or geographical map visualisations** may be omitted. A static presentation with the above-mentioned TEI Publisher plug-in from Eleventy is limited to simple searches, i.e. the possibility of a [faceted search](https://en.wikipedia.org/wiki/Faceted_search), as made possible by databases, is restricted or requires a more technically sophisticated preparation of the search index. Visualisation tools that have to rely on external resources can be integrated into a static presentation, but their functioning depends on the external resource.

## Limitations of Data formats for the static presentation

In the following, HTML and JSON are presented as the two most important data formats into which TEI/XML data must be converted for static presentations. This section is primarily aimed at technically trained editors.

### HTML-based presentations

The **most radical implementation** is a conversion of the edition data into HTML files, which are as static as a printed book.
Content and form are no longer separated in this form.
With HTML, the data is in a long-lasting format that can also be used offline in the web browser without any effort.

The disadvantage is that different views of the same content have to be converted separately and are given separate paths for each file.
The **linking** between different contents is therefore directly linked to the conversion and must be taken into account during revisions.

In addition, **search functions** are not possible in pure HTML presentations without a database, so you have to rely on external providers such as search engines or pursue a hybrid approach in which individual views such as the search are implemented in JavaScript.

HTML-based editions must be developed as such from the ground up.
XSLT conversions can be used as a tool.

==->@How sustainable is an XSLT conversion on the fly in the browser?

### JSON-based presentations

Less radical is the use of JSON files with the content equivalent to the data from the database interface. HTML is only used as a format for the individual properties.
The conversion of existing presentations into static ones is also possible **relatively late** with this approach and the dynamic user experience can be preserved.

A disadvantage is the **dependence on fast-moving JavaScript libraries** (especially for full-text search) and that the edition can only be used on the local computer via HTTP.

**Search functions** can be executed via libraries such as [FlexSearch](https://github.com/nextapps-de/flexsearch){:target="\_blank"} can be executed in the browser.
The data format of the index data follows the respective library and a conversion corresponds to a new implementation. Loading the search index leads to more data traffic with large data sets.
