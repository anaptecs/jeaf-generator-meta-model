---
title: "UML Modeling Guide"
subtitle: "Stereotype «HeaderParam»"
toc: false
menubar: jmm_menu
---

# Stereotype `«HeaderParam»`
Stereotype `«HeaderParam»` is used to mark that a parameter of a REST operation should be taken from the http header. Please be aware that the stereotype can only be applied on an operation of an interface that is marked as `«RESTResource»` and the operation is marked as `«RESTOperation»`.

<br>

| **Stereotype**          | `«HeaderParam»` | |
| ----------------------- | -------------- | |
| **Applicable Elements** | `Parameter` `Property`        |
| **Tagged Values**       |                       |                                                                                                                                                                                                          |
| **Name**                | **Type**              | **Description**                                                                                                                                                                                          |
| `value`   | `String` | Name of the http header field from which the parameter value should be taken. |
| `technicalHeader`   | `Boolean` | If a header field is marked as a technical header then it will be part of the published API e.g. in the OpenAPI specification. However it will be hidden to the generated business code. |

<br>

For further information please refer to: 
- [`«REST Resource»`](/uml-modeling-guide/jmm/RESTResource) 
- [`«REST Operation»`](/uml-modeling-guide/jmm/RESTOperation) 
- [How to model REST Services](/uml-modeling-guide/how-tos/how-to-model-rest-service-apis) 
- [Generating Code for REST Services](/developer-guide/code-for-jeaf-services)


<br>

<div style="text-align: right"><code>Generated by JEAF Generator</code></div>

    