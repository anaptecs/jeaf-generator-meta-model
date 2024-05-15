---
title: "UML Modeling Guide"
subtitle: "Stereotype «RESTOperation»"
toc: false
menubar: jmm_menu
---

# Stereotype `«RESTOperation»`
Stereotype `«RESTOperation»` is used to mark that an operation of a service should also be accessible via REST. 

Please be aware that the stereotype can only be applied on an operation of an interface that is marked as «JEAFService».

<br>

| **Stereotype**          | `«RESTOperation»` | |
| ----------------------- | -------------- | |
| **Applicable Elements** | `Operation`        |
| **Tagged Values**       |                       |                                                                                                                                                                                                          |
| **Name**                | **Type**              | **Description**                                                                                                                                                                                          |
| `path`   | `String` | Path under which the REST resource should be available. The attribute is optional in case that a path is already defined for the REST resource. |
| `httpMethods`   | `HTTPMethod` | HTTP methods that are used to request the operation. At least one method must be defined. |
| `produces`   | `MediaType` | Optional definition of the media types that are used to encode the responses of the REST calls (e.g. JSON, XML etc.). |
| `consumes`   | `MediaType` | Optional definition of the media types that are supported to be used to encode REST requests (e.g. JSON, XML etc.). |
| `statusCode`   | `HTTPStatusCode` | Status code that will be used in case that the REST call was successful. |
| `async`   | `Boolean` | Attribute defines if the processing of the REST request will be asynchronous or not. This will not have any impact on the REST client but on the generated implementation of the REST operation itself. |
| `externalDocsURL`   | `String` | Link to additional external documentation about an operation. |
| `operationID`   | `String` | OpenAPI operationID |
| `summary`   | `String` | Summary documentation of the operation for openAPI specification only. |

<br>

For further information please refer to:
- [How to model REST Services](/uml-modeling-guide/how-tos/how-to-model-rest-service-apis)
- [Generating Code for REST Services](/developer-guide/code-for-jeaf-services)


<br>

<div style="text-align: right"><code>Generated by JEAF Generator</code></div>

    