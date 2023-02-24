---
title: CreateLookupTaskDefinition
second_title: Aspose.Tasks voor .NET API-referentie
description: Fabrieksmethode die een uitgebreide attribuutdefinitie creëert met lookup. Het heeftCalculationTypeaspose.tasks/extendedattributedefinition/calculationtype/ is gelijk aanLookup en kan alleen in Tasks worden gebruikt. U bent verplicht om op te gevenfieldId Enalias wanneer deze methode wordt aangeroepen. Het veldtype wordt afgeleid uit veldid.
type: docs
weight: 20
url: /nl/net/aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/
---
## CreateLookupTaskDefinition(ExtendedAttributeTask, string) {#createlookuptaskdefinition_1}

Fabrieksmethode die een uitgebreide attribuutdefinitie creëert met lookup. Het heeft[`CalculationType`](../calculationtype/) is gelijk aanLookup en kan alleen in Tasks worden gebruikt. U bent verplicht om op te geven*fieldId* En*alias* wanneer deze methode wordt aangeroepen. Het veldtype wordt afgeleid uit veld-id.

```csharp
public static ExtendedAttributeDefinition CreateLookupTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | De opgegeven[`ExtendedAttributeTask`](../../extendedattributetask/) veld ID. |
| alias | String | De opgegevenString alias. |

### Winstwaarde

Gemaakt exemplaar van de[`ExtendedAttributeDefinition`](../) klasse met opgegeven*fieldId* En*alias*.

### Voorbeelden

Gebruik dit voorbeeld om een aangepaste velddefinitie te maken voor een taak met opzoeken en deze vervolgens te vullen met tekstwaarden:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
taskTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(taskTextAttr);
```

### Zie ook

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* naamruimte [Aspose.Tasks](../../extendedattributedefinition/)
* montage [Aspose.Tasks](../../../)

---

## CreateLookupTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createlookuptaskdefinition}

Fabrieksmethode die een uitgebreide attribuutdefinitie creëert met lookup. Het heeft[`CalculationType`](../calculationtype/) is gelijk aanLookup en kan alleen in Tasks worden gebruikt. U bent verplicht om op te geven*customFieldType* ,*fieldId* En*alias* wanneer deze methode wordt aangeroepen.

```csharp
public static ExtendedAttributeDefinition CreateLookupTaskDefinition(
    CustomFieldType customFieldType, ExtendedAttributeTask fieldId, string alias)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| customFieldType | CustomFieldType | De opgegeven[`CustomFieldType`](../../customfieldtype/) type. |
| fieldId | ExtendedAttributeTask | De opgegeven[`ExtendedAttributeTask`](../../extendedattributetask/) veld ID. |
| alias | String | De opgegevenString alias. |

### Winstwaarde

Gemaakt exemplaar van de[`ExtendedAttributeDefinition`](../) klasse met opgegeven*customFieldType* ,*fieldId* En*alias*.

### Voorbeelden

Gebruik dit voorbeeld om een aangepaste velddefinitie te maken voor een taak met opzoeken en deze vervolgens te vullen met tekstwaarden:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
taskTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(taskTextAttr);
```

### Zie ook

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* naamruimte [Aspose.Tasks](../../extendedattributedefinition/)
* montage [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->