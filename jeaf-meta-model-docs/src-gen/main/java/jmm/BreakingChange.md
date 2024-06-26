---
title: "UML Modeling Guide"
subtitle: "Stereotype «BreakingChange»"
toc: false
menubar: jmm_menu
---

# Stereotype `«BreakingChange»`
Stereotype `«BreakingChange»` can be used to mark model elements that are a breaking change compared to a previous version.

This is especially useful when you are working with semantic versioning approach. Using this stereotype you can then mark elements that break backward compatibility.

Example: a new request property is introduced and after a transition phase it will be mandatory.

JEAF Generator supports a so called breaking changes report that lists all the breaking changes.
 

<br>

| **Stereotype**          | `«BreakingChange»` | |
| ----------------------- | -------------- | |
| **Applicable Elements** | `NamedElement`        |
| **Tagged Values**       |                       |                                                                                                                                                                                                          |
| **Name**                | **Type**              | **Description**                                                                                                                                                                                          |
| `description`   | `String` | Description of an upcoming breaking change. |
| `activeWith`   | `String` | Version when a breaking change becomes active. <br><br>**Example:**<br>- A new parameter is introduced for a request. To not immediately break the API at first the parameter is optional. Using this field it can be defined when the parameter will be mandatory. |
| `breakingChangeType`   | `BreakingChangeType` | Type of the breaking change. <br><br>Currently the following types of breaking changes are supported:<br>* `DEPRECATION_EXPIRED`: some functionality (e.g. an operation or property) will be removed after it was deprecated<br>* `RUNTIME_COMPATIBLE_ONLY`: A breaking change occurs only on code level but not at runtime. An example for such cases could be that the responses of a REST service is still backward compatible on a JSON level, but if the new version of generated classes is used then compile errors will occur (e.g. because of moving classes to a different package)<br>* `JOINED_DEPLOYMENT_REQUIRED`: Breaking changes of this type require a joined deployment / update of all parts at the same time :unamused: |



<br>

<div style="text-align: right"><code>Generated by JEAF Generator</code></div>

    