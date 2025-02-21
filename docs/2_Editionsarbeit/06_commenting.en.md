# 2.5 Commentary

## Forms of Commentary in DSE

In both printed and digital editions, the commentary allows texts to be enriched with contextual information beyond text-critical and content annotations. Commentaries are typically the result of research, whether it involves research closely tied to the [_constitution of text_](02_Textkonstitution.en.md) that doesn't require significant additional effort, or research conducted in parallel with the edition project as independent scholarly work, which may also be repurposed in essays or monographs.

In traditional print editing, three basic forms of commentary are recognized, all of which are also used in different forms within DSE:

**1. The editorial commentary** (also known as the editor's commentary, editorial report, etc.) explains at least the editorial guidelines, possibly the selection of the corpus based on its genesis, and the use of the text-critical apparatus. In DSE, this form of commentary is more commonly referred to as [_documentation_](../3_presentation/04_documentation.en.md) and will be discussed under this name in the Publication chapter.

!!! info "Exemplary DSE"
    
    In hybrid editions such as the [Faustedition](https://www.faustedition.net/), the editorial report (which applies to both the digital and printed editions) and the technical documentation are sometimes separated.

**2. The overview commentary** (also known as the introductory commentary, contextual essay, or commentary on the entire text) refers to the edited content as a whole, whether it's a specific subject area, a group of works, or a single text. In historical-critical editions, it often serves to summarize content (called a _regest_ in the case of historical source editions and letter editions), illuminate its genesis (text genesis, intertextuality), publication history, reception, and sometimes even offer an overview of interpretations in the secondary literature. Various forms of overview commentaries also exist in DSE. However, these are rarely compiled into one continuous text, but instead appear at different hierarchical levels closer to the annotated content (e.g., an introduction to the Letters section, an introduction to a specific correspondence, individual letter commentaries). Since these are individual texts loosely connected to the edited text (which, ideally, can be output as TEI/XML just like the edited text), the technical and editorial aspects are less complex and don't need further elaboration.

!!! info "Exemplary DSE"
    
    The overview commentaries of the [edition humboldt digital](https://edition-humboldt.de) are exemplary, as they provide a separate introduction for each letter correspondence (a similar approach is followed by the later letter editions in [haller.net](https://hallernet.org). In addition to such an "introduction", each of Humboldt's individual travel diaries also contains "research dossiers", some of which exceed traditional overview commentaries in their level of detail. This enrichment of the edition through thematic essays can demonstrate its research value. Finally, edition humboldt digital sometimes also includes a detailed overview commentary at the level of individual texts. This commentary is called "Anmerkung" and appears as hover/mouseover text when the metadata is accessed. It is primarily concerned with the dating and structure of the individual document. Branching into various overview commentaries is unnecessary in the case of a single edited text, such as a novel. Therefore, the [overview commentary of the Lokalbericht Edition](https://www.lokalbericht.ch/kommentar) is structured as a continuous text, closely linked to individual sections of the edition.

**3 The passage commentary** refers to a single text passage, the length of which can range from a single word to passages spanning several paragraphs. Printed editions are familiar with the practice of commenting on passages either in close proximity to the text (in the margin, as a footnote) or in a commentary apparatus (structured by endnotes, line numbers, and/or lemmata). Digital scholarly editions (DSE) have the advantage here of being able to link passage commentaries more directly to the annotated content. Various methods for creating digital passage commentaries are explored in more detail below.

## Workflows for Passage Commentaries

At this point, it’s not yet possible to speak of 'standard workflows' as in the other chapters on editing work, since editions have **very different needs** when it comes to annotating passages and often forgo them entirely. The need for passage commentaries has decreased in comparison to print editions, as many of them can now be replaced by [_content annotations_](05_semantic_annotation.en.md).

However, when passage commentaries are created, their 'anchoring' or coding in TEI-XML is quite standardized, as they are typically inserted as `<note>` for simplicity. => You might want to insert a code snippet from the showcase edition here, or better yet, link directly to the TEI-XML.

The TEI/XML coding, however, does not specify **how the passage commentary will ultimately be displayed**. This depends on the choice of ODD and the technology of the publication tool. In the case of the TEI Publisher, passage commentaries are currently displayed as endnotes beneath the edited text. The endnote anchor in the body text is linked to the endnote (as commonly seen in Word documents), so that when clicked, the page scrolls to the corresponding endnote. For the Showcase Edition, we've enhanced this functionality so that a hover/mouseover text appears when the cursor is placed over the endnote anchor.

![Commenting in TEI Publisher in endnotes with TEI-XML](image-5.png)

Since passage comments are simple **to handle as annotations** in the code, they can be inserted using the annotation editor in the TEI Publisher. However, at present, they cannot be deleted using the standard configuration in the editor, meaning they must be manually removed from the TEI/XML file. To minimize the need for constant work in TEI/XML, the Showcase Edition has decided to initially mark such deletions with a TODO annotation and execute them in bulk later.

For consistent use of passage commentaries, it makes sense to document these in the editing guidelines.

!!! abstract "Showcase Edition Guidelines: Commentary"
    
    => @ Ursula: We have not yet defined actual commentary guidelines, commenting is primarily your area of expertise. Why should what be commented on and when?
