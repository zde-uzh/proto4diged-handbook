# 3.1 Access points: Pages, searches and indexes

The form of access depends on the **intended audience** that the DSE wants to address (or implicitly does not want to address). Within DSE projects, there are sometimes lively discussions about how strongly access to the edition should be structured, in particular whether the entry point should first provide an introduction to the use of the edition and/or its subject before texts or other media are made accessible, or whether various access points should be presented as intuitively and quickly as possible.

We favour **low-threshold forms** of access and will attempt to evaluate these in the following using concrete examples. We do not deny that 'upstream' introductions are justified, especially as they can serve to reduce the threshold; for example, in older DSEs, functions that are now taken for granted by many users still require explanation. Furthermore, low-threshold does not mean that all access to the edition is already provided on the entry page (see below); this can also appear confusing and make it more difficult to get started.
In addition to various forms of entry pages, various search functions and indexes are central to accessing the edited texts, which is why they are also dealt with below.


## Entry pages

A distinction can be made between two basic concepts of entry pages:

1. **Introductions to the edited material**, i.e. access to various resources and indexes is prioritised and the path to them is immediately visible.

!!! info "Exemplary DSE: Standard entry page to the DSE"
    The standard example is the main page of the TEI Publisher, which lists all texts in alphabetical or numerical order.

    - For example, after a very simple introductory page that briefly outlines the project, the [Coseriu Edition](https://coseriu.uzh.ch/static/home.xml){:target="\_blank"} main page provides an overview of all texts, which makes sense given the rather small volume of correspondence. The St Gallen [Missive Edition](https://missiven.stadtarchiv.ch/start.html){:target="\_blank"} takes a similar approach. .
    - The homepage of the [Escher Letter Edition](https://www.briefedition.alfred-escher.ch/home.html){:target="\_blank"}  is somewhat more complex, but remains clear and also allows access to the text selection with one click.

    Typical of many editions in the TEI Publisher is that the **search field and the index menu** (sometimes as 'Contexts') are always visible from the start page.

2 **Introduction to the project**, i.e. the description of the project framework, usage and, if applicable, access to the documentation is of primary or equal importance. The path to the edited text often only becomes clear after reading the introductory page and/or runs over several sub-pages.

!!! info "Exemplary DSE: Getting started with the project"
    Particularly if an edition only has a few edited documents, an introduction to the project can clarify from the outset that it is an unfinished 'work in progress'. An edition of very specialised, complexly structured holdings, which, for example, have the function of a digital archive, can also justify a detailed introduction.

    - One example of this is the [Niklas Luhmann Archive](https://niklas-luhmann-archiv.de){:target="\_blank"} whose core consists of an edition of the scientist's card index and working typescripts or manuscripts. Since even complex analogue working tools had to be translated into digital form, the edition features [reading paths](https://niklas-luhmann-archiv.de/bestand/zettelkasten/lesewege){:target="\_blank"} and [tutorials](https://niklas-luhmann-archiv.de/bestand/zettelkasten/tutorial){:target="\_blank"}, which are presented at least as equally as the edition text itself.

    - There are examples of extensive introductions in the TEI Publisher, such as [Louis Ginzberg's "Legend of the Jews"](https://www.ginzberg.ethz.ch/index.html){:target="\_blank"} which comprises two main pages ("About the Edition" and "Edition") and shows the 'About' page first.

In both scenarios, users should quickly realise what the edition is and who made it. When developing specific web design, attention should be paid to simplicity and good comprehensibility on the entry page. This significantly supports [_Accessibility_](../themes/accessibility.en.md), which we will discuss in more detail in this manual.

The initial page of the TEI Publisher can be **configured**, as described in detail in the [TEI Publisher documentation]. => @Reto I have not yet found the relevant documentation.

The Showcase edition also provides its entry page - which largely corresponds to the standard settings - as source code: => Link to Github here when we are ready.

## Search functions

The more complex the edition, the more search functions are useful. In addition to the main function - the full-text search in the edited text - a targeted search in the commentaries, indexes or bibliographies can be useful. The [edition-humboldt](https://edition-humboldt.de/){:target="\_blank"} offers an exemplary selection. However, these functions are not necessary where hardly any comments are used and indexes can simply be browsed in a short time.
=> @ Reto: Are there any technical aspects to add to the TEI Publisher?

## Registers and maps

In addition to a list of documents and the search function, indexes are the most important access point to the edition. As already seen in connection with the [_content annotation_](../2_Editionsarbeit/05_semantic_annotation.en.md), the most common indexes are those for persons, keywords and places. The latter indexes can be supplemented with maps, which also allow the location data to be graphically assigned and located.  

!!! info "Exemplary DSE: Simple indexes"
    **Simple indexes** are usually organised alphabetically by entry (place name, surname of a person etc.); this also applies to the standard indexes in the TEI Publisher (below is the example of the name indexes of the St.Gallen Missives Edition).
    ![Name register of missives](image-4.png){ width="1000" }
    <figcaption> Index of persons of the DSE "Briefverkehr der Stadt St. Gallen 1400-1650. Digitale Missivenedition", [https://missiven.stadtarchiv.ch/namen/?search=&category=A]([https://missiven.stadtarchiv.ch/namen/?search=&category=A){:target="\_blank"}. Retrieved on 24.9.2024.</figure>

!!! info "Exemplary DSE: More complex registers"
    **More complex registers** such as that of [hallernet](https://hallernet.org/){:target="\_blank"} which are not created with standard tools, also allow dynamic adjustments to the order, for example by allowing personal entries to be sorted according to place of birth and place of death. hallernet emphasises the networking of its databases and has the character of a research database, which is why the various registers are also in the foreground on the homepage.
    ![Person register hallernet](image-3.png) <figcaption>Person register of the platform "hallernet", [https://hallernet.org/data/persons?query=&scope=mt&filters=]([https://hallernet.org/data/persons?query=&scope=mt&filters=){:target="\_blank"}. Retrieved on 24.9.2024.</figure>

!!! info "Exemplary DSE: Simple register entry"
    Each **register entry** is linked to a specific register page. Like the register itself, this can vary in complexity; in the standard case (which also applies to the TEI Publisher), all occurrences of the entry in the edition as well as a link to resources and standardisation data entries outside the edition** are listed on a register page (below is an example of a name register page of the missives edition).
    ![Name index page of the missives edition](image-6.png){ width="1000" }
    <figcaption> Name index page of the DSE "Briefverkehr der Stadt St. Gallen 1400-1650. Digitale Missivenedition", [https://missiven.stadtarchiv.ch/namen/Brandenburg,%20Friedrich%20I.%20von%20(1438%E2%80%93)?&category=B&search=&key=stadtasg-actors-240]([https://missiven.stadtarchiv.ch/namen/Brandenburg,%20Friedrich%20I.%20von%20(1438%E2%80%93)?&category=B&search=&key=stadtasg-actors-240){:target="\_blank"}. Retrieved 24.9.2024.</figure>

!!! info "Exemplary DSE: Complex register entry"
    Where, as in [hallernet](https://hallernet.org/){:target="\_blank"}, the database structure is central, register pages can also be enriched with further information about the entity, e.g. in the case of a person, metadata about publications or professional functions. Such 'haute couture' solutions require a **complex database in the background** and corresponding technical expertise in the creation and maintenance of databases.
        ![Person register page hallernet](image-5.png) <figcaption> Name register page of the DSE "hallernet", [https://hallernet.org/data/person/28859](https://hallernet.org/data/person/28859){:target="\_blank"}. Accessed on 24.9.2024.</figure>

## Timeline

Although time data also belongs to the standard category of content markup, it is usually not displayed as a tab, but as [_timelines_](04_timelines_maps.en.md). The TEI Publisher allows this timeline to be displayed on the main page. The St. Gallen [Missive Edition](https://missiven.stadtarchiv.ch/start.html?query=&subtype=document&dates=&collection=&start=1){:target="\_blank"}, for example, makes use of this solution. makes use of this solution.

