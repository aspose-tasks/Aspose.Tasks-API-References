---
title: AddLookupValue
second_title: Aspose.Tasks for .NET API Reference
description: आंतरक लुकअप सूच में मन जड़त है के सथ हेरफेर करने क यह एक बेहतर तरक हैValueListaspose.tasks/extendedattributedefinition/valuelist/ .
type: docs
weight: 290
url: /hi/net/aspose.tasks/extendedattributedefinition/addlookupvalue/
---
## ExtendedAttributeDefinition.AddLookupValue method

आंतरिक लुकअप सूची में मान जोड़ता है। के साथ हेरफेर करने का यह एक बेहतर तरीका है[`ValueList`](../valuelist/) .

```csharp
public void AddLookupValue(Value value)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | Value | लुकअप में जोड़ने के लिए मान। |

### टिप्पणियों

यह तरीका केवल के लिए काम करता है[`ExtendedAttributeDefinition`](../) उदाहरण जिनके पास है[`CalculationType`](../calculationtype/) बराबर हैLookup .

### उदाहरण

लुकअप सूची में नया मान जोड़ने के लिए इस कोड का उपयोग करें:

```csharp
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
```

### यह सभी देखें

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* नाम स्थान [Aspose.Tasks](../../extendedattributedefinition/)
* सभा [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->