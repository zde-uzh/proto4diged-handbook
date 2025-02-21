# 2.3 Conversion from PAGE to TEI

## 1. Why Convert?

As previously mentioned in connection with transcription, ALTO and PAGE XML are ATR standards. They produce one XML document per transcribed page, whereas TEI/XML can contain an unlimited number of pages. TEI allows content-oriented structures and multiple sources within a single document, while PAGE only represents the facsimile. TEI/XML is thus the edition standard that enables editions of any length to be annotated and published. All XML formats are machine-readable, but TEI/XML is also easier for humans to read and manipulate. This is why DSE projects have the option to prepare their TEI/XML data directly in XML editors such as [Oxygen](https://www.oxygenxml.com/){:target="\_blank"}. Conversion is still necessary in this case as well.

## 2. Standard Conversion Options

### Transkribus (Exports)

Transkribus offers a variety of export options (PDF, Textfile, Docx, Excel/CSV, PAGE-XML, ALTO-XML, TEI/XML); however, only the last three can be used for the development of a DSE according to current standards. While PAGE-XML and ALTO-XML still need to be converted into TEI/XML, the TEI/XML provided by a Transkribus export unfortunately does not yet meet the desired quality. If many custom tags have been assigned in Transkribus, the export must therefore be revised.

### eScriptorium (PAGE, ALTO)

eScriptorium currently has two export options: PAGE-XML and ALTO-XML.

### Existing Scripts (trans2tei, page2tei)

Because exports in TEI XML format are either missing or insufficient in common transcription tools, code scripts have been developed in recent years to avoid manual conversion (e.g., in an XML editor like Oxygen). The two scripts presented here automate the conversion process.

The basic script is [**page2tei**](https://github.com/dariok/page2tei), which converts PAGE-XML into TEI/XML.
The biggest obstacle with page2tei is a TODO for line tags. Once this is resolved, custom conversion can be done as the next step (cascade). Other edition-specific tags are placed in anonymous blocks (tag ab) with a type attribute, which can be processed effectively.

[**trans2tei**](https://github.com/biblhertz/trans2tei){:target="\_blank"} is specifically tailored to PAGE XML output from Transkribus. It includes all steps from the export zip to TEI-XML and also covers the recognition of printed highlights using special characters. trans2tei is aimed at the needs of the Bibliotheca Herziana. For edition projects, it is best used simply as inspiration.

=> The proto2tei script, which is tailored to the Showcase edition, will appear here later.

## 3. Limitations

If no or only a minimal tag set is available, the TEI-XML export from Transkribus requires little to no readjustment. However, in this case, an important function of the tool is lost: the annotation of text or text regions.

To address this issue, **manual readjustments** can be made to ensure conformity with the desired TEI schema. Depending on the complexity of the schema, such manual revisions can become time-consuming.

Ultimately, with sufficient technical expertise, project-specific conversions can be developed using pipelines such as [trans2tei](https://github.com/biblhertz/trans2tei){:target="\_blank"}.
The basis for this is [page2tei](https://github.com/dariok/page2tei){:target="\_blank"}, which is already available in Transkribus's export function.
