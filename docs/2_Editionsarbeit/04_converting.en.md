# 2.3 Conversion from PAGE to TEI

## 1. Why conversion?

As already described in connection with transcription, ALTO and PAGE XML are ATR standards. They output one XML document per transcribed page, unlike TEI/XML, which can contain an unlimited number of pages. TEI allows content-orientated structures and several sources in one document, PAGE only displays the facsimile. TEI/XML is therefore the edition standard that allows editions of any length to be annotated and published. All XML formats are machine-readable, TEI/XML is also easier for humans to read and manipulate, which is why DSE projects also have the option of preparing their TEI/XML data directly in XML editors such as [Oxygen](https://www.oxygenxml.com/){:target="\_blank"}. Conversion is also necessary in the latter case.

## 2. standard conversion options

### Transkribus (exports)

Transkribus offers a variety of export options (PDF, Textfile, Docx, Excel/CSV, PAGE-XML, ALTO-XML, TEI/XML); however, only the last three can be used for the development of a DSE according to current standards. While PAGE-XML and ALTO-XML themselves still need to be converted into TEI/XML, the TEI/XML provided by a Transkribus export unfortunately does not yet meet the desired quality. If many custom tags have been assigned in Transkribus, the export must therefore be revised.


### eScriptorium (PAGE, ALTO)

eScriptorium currently has two export options: PAGE-XML and ALTO-XML.

### Existing scripts (trans2tei, page2tei)

Because exports in TEI XML format are either missing or insufficient in the common transcription tools, code scripts have been developed in recent years to avoid manual conversion (e.g. in an XML editor such as Oxygen). The two scripts presented here automate the conversion.

The basic script is [**page2tei**](https://github.com/dariok/page2tei), which converts PAGE-XML into TEI/XML.
The biggest obstacle with page2tei is a TODO for line tags. Once this is solved, the custom conversion can be done as the next step (cascade). Other edition-specific tags are placed in anonymous blocks (tag ab) with a type attribute, which can be processed in the best possible way.

[**trans2tei**](https://github.com/biblhertz/trans2tei){:target="\_blank"} is specifically tailored to PAGE XML output from Transkribus. It includes all steps from export zip to TEI-XML and also covers the recognition of printed highlighting using special characters.
trans2tei is aimed at the needs of the Bibliotheca Herziana. For editing projects, it is best used simply as an inspiration.

=> The proto2tei script, which is tailored to the Showcase edition, will appear here later.

## 3. limitations

If no or only a minimal tag set is available, the TEI-XML export of Transkribus requires hardly any readjustment. In this case, however, an important function of the tool is omitted: the annotation of text or text regions.

Even more serious is the fact that the **reference to the facsimile**, which is now a standard feature of many DSEs, is missing, as the coordinates are also omitted in this case.

As a solution to this problem, **manual readjustments** can be carried out in order to achieve conformity with the desired TEI schema. However, such manual revisions can be time-consuming depending on the complexity of the schema.

Ultimately, with sufficient technical expertise, project-specific conversions can be developed using pipelines such as [trans2tei](https://github.com/biblhertz/trans2tei){:target="\_blank"}  can be developed.
The basis for this is [page2tei](https://github.com/dariok/page2tei){:target="\_blank"}, which is already available in the Transkribus export function.
