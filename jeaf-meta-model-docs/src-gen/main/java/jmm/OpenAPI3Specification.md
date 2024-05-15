---
title: "UML Modeling Guide"
subtitle: "Stereotype «OpenAPI3Specification»"
toc: false
menubar: jmm_menu
---

# Stereotype `«OpenAPI3Specification»`
Stereotype `«OpenAPI3Specification»` can be used to mark a component as OpenAPI 3 specification. This element represents the specification document that will be generated by JEAF Generator.

<br>

| **Stereotype**          | `«OpenAPI3Specification»` | |
| ----------------------- | -------------- | |
| **Applicable Elements** | `Component`        |
| **Tagged Values**       |                       |                                                                                                                                                                                                          |
| **Name**                | **Type**              | **Description**                                                                                                                                                                                          |
| `resourceName`   | `String` | Name of the file that will be generated as OpenAPI specification file. By default it will be named as `openapi.yml`. |
| `apiVersion`   | `String` | Version of the API that is represented by this OpenAPI specification. We strongly recommend to version you API according to the rules of [Semantic Versioning](https://semver.org). |
| `contactName`   | `String` | Name of the team or person that will be mentioned in your OpenAPI specification as contact. |
| `contactURL`   | `String` | URL of the contact for your OpenAPI specification. |
| `contactEmail`   | `String` | Email of the contact that is mentioned in your OpenAPI specification. |
| `licenseName`   | `String` | Name of the license under which your OpenAPI specification is published e.g. `Apache 2.0`. |
| `licenseURL`   | `String` | URL under which the used license is available. |
| `termsOfUseURL`   | `String` | URL under which the terms of use are published. |
| `securityOptional`   | `Boolean` | Tagged value can be used to define that the security section of the OpenAPI specification will not be provided. |
| `explicityTypeOrdering`   | `Boolean` | By default types are ordered in an alphabetic order. However, JEAF Generator also supports to define an explicit type ordering in OpenAPI specifications. <br><br>This can be enabled using this tagged value. In addition stereotype «Ordered» has to be applied on the elements of the OpenAPI Types that belong to the OpenAPI specification. |
| `explicitPathOrdering`   | `Boolean` | As for types it is also to define an explicit order for paths. <br><br>This can be enabled using tagged value. In addition stereotype «Ordered» has to be applied on the REST operations that belong to the OpenAPI specification. |

<br>

For further information please refer to:
- [How to publish REST Services as OpenAPI 3 specification](/uml-modeling-guide/how-tos/how-to-model-open-api)
- [Generating OpenAPI Specification](/developer-guide/generating-open-api-spec)


<br>

<div style="text-align: right"><code>Generated by JEAF Generator</code></div>

    