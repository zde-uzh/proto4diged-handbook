# Annotations with TEI Publisher

TEI Publisher offers a basic configuration for the annotation of XML data, ranging from pure layout annotations to linking with register entries and the creation of a register.
The supplied configuration can be used directly or serve as an example for extensions to meet the needs of a project.

The underlying XML file is transferred to a specific HTML format and the spaces are analysed so that annotations can be inserted in the correct position.

## Customisations

As the annotation view is based on the same technology as the presentation, the customisation is similar to that of the edition views.

## Limitations

Particularly for annotation with a link to the register, there are a number of mechanisms in operation in the background which, for example, favour local entries, prioritise more frequent annotation and so on, which must be taken into account when making adjustments. Experience with TEI Publisher is therefore a prerequisite.

Other limitations include internal dependencies in folders whose modification is not recommended ([Best Practice Recommendations](https://teipublisher.com/exist/apps/tei-publisher/documentation/customization-best-practice#){:target="\_blank"}) or dependencies on values in the web components ([Webcomponent Documentation](https://teipublisher.com/exist/apps/tei-publisher/documentation/webcomponents-docs){:target="\_blank"}, cf. also [Changing and Debugging Web Components](https://faq.teipublisher.com/webcomponents/debug/){:target="\_blank"}, [Creating Custom Web Components](https://teipublisher.com/exist/apps/tei-publisher/documentation/custom-components#){:target="\_blank"}), if, for example, a standard data API is not supported or a complex annotation requires special functionalities for editing or deletion.

## Documentation

The following chapter of the documentation is relevant for all editorial staff:

- [Annotating Documents](https://teipublisher.com/exist/apps/tei-publisher/documentation/web-annotations){:target="\_blank"}

The following chapters are also relevant for technical staff:

- [Configuring the Annotation Editor](https://teipublisher.com/exist/apps/tei-publisher/documentation/configuring-annotation-editor){:target="\_blank"}

- [Local authority registers](https://teipublisher.com/exist/apps/tei-publisher/documentation/registers){:target="\_blank"}
