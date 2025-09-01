# Annotations with TEI Publisher

TEI Publisher provides a basic configuration for annotating XML data, ranging from pure layout annotations to linking with index entries and creating an index.
The supplied configuration can be used directly or as an example for extensions tailored to a project's specific needs.

The underlying XML file is converted into a specific HTML format, and spaces are analyzed so that annotations can be inserted at the correct positions.

## Customizations
Since the annotation view is based on the same technology as the presentation, customizations are similar to those of the edition views.

## Limitations
Particularly when annotating with links to the index, there are several mechanisms running in the background. For instance, they may prioritize local entries, give preference to more frequent annotations, and so on. These factors need to be considered when making adjustments. Experience with TEI Publisher is therefore a prerequisite.

Other limitations include internal dependencies in folders whose modification is not recommended ([Best Practice Recommendations](https://teipublisher.com/exist/apps/tei-publisher/documentation/customization-best-practice#){:target="\_blank"}) or dependencies on values in the web components ([Webcomponent Documentation](https://teipublisher.com/exist/apps/tei-publisher/documentation/webcomponents-docs){:target="\_blank"}, cf. also [Changing and Debugging Web Components](https://faq.teipublisher.com/webcomponents/debug/){:target="\_blank"}, [Creating Custom Web Components](https://teipublisher.com/exist/apps/tei-publisher/documentation/custom-components#){:target="\_blank"}), if, for example, a standard data API is not supported or a complex annotation requires special functionalities for editing or deletion.

## Documentation

The following chapter of the documentation is relevant for all editorial staff:

-   [Annotating Documents](https://teipublisher.com/exist/apps/tei-publisher/documentation/web-annotations){:target="\_blank"}

The following chapters are also relevant for technical staff:

-   [Configuring the Annotation Editor](https://teipublisher.com/exist/apps/tei-publisher/documentation/configuring-annotation-editor){:target="\_blank"}

-   [Local authority indexes](https://teipublisher.com/exist/apps/tei-publisher/documentation/registers){:target="\_blank"}
