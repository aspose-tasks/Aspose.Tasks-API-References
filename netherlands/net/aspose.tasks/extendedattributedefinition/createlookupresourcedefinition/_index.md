---
title: CreateLookupResourceDefinition
second_title: Aspose.Tasks voor .NET API-referentie
description: Fabrieksmethode die een uitgebreide attribuutdefinitie creëert met lookup. Het heeftCalculationTypeaspose.tasks/extendedattributedefinition/calculationtype/ is gelijk aanLookup en kan alleen in Resources worden gebruikt. U bent verplicht om te specificerenfieldId Enalias wanneer deze methode wordt aangeroepen. Het veldtype wordt afgeleid uit veldid.
type: docs
weight: 10
url: /nl/net/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---
## CreateLookupResourceDefinition(ExtendedAttributeResource, string) {#createlookupresourcedefinition_1}

Fabrieksmethode die een uitgebreide attribuutdefinitie creëert met lookup. Het heeft[`CalculationType`](../calculationtype/) is gelijk aanLookup en kan alleen in Resources worden gebruikt. U bent verplicht om te specificeren*fieldId* En*alias* wanneer deze methode wordt aangeroepen. Het veldtype wordt afgeleid uit veld-id.

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | De opgegeven[`ExtendedAttributeResource`](../../extendedattributeresource/) veld ID. |
| alias | String | De opgegevenString alias. |

### Winstwaarde

Gemaakt exemplaar van de[`ExtendedAttributeDefinition`](../) klasse met opgegeven*fieldId* En*alias*.

### Voorbeelden

Gebruik dit voorbeeld om een aangepaste velddefinitie te maken voor een resource met opzoeken en deze vervolgens te vullen met tekstwaarden:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Zie ook

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* naamruimte [Aspose.Tasks](../../extendedattributedefinition/)
* montage [Aspose.Tasks](../../../)

---

## CreateLookupResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createlookupresourcedefinition}

Fabrieksmethode die een uitgebreide attribuutdefinitie creëert met lookup. Het heeft[`CalculationType`](../calculationtype/) is gelijk aanLookup en kan alleen in Resources worden gebruikt. U bent verplicht om te specificeren*customFieldType* ,*fieldId* En*alias* wanneer deze methode wordt aangeroepen.

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    CustomFieldType customFieldType, ExtendedAttributeResource fieldId, string alias)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| customFieldType | CustomFieldType | De opgegeven[`CustomFieldType`](../../customfieldtype/) type. |
| fieldId | ExtendedAttributeResource | De opgegeven[`ExtendedAttributeResource`](../../extendedattributeresource/) veld ID. |
| alias | String | De opgegevenString alias. |

### Winstwaarde

Gemaakt exemplaar van de[`ExtendedAttributeDefinition`](../) klasse met opgegeven*customFieldType* ,*fieldId* En*alias*.

### Voorbeelden

Gebruik dit voorbeeld om een aangepaste velddefinitie te maken voor een resource met opzoeken en deze vervolgens te vullen met tekstwaarden:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Zie ook

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* naamruimte [Aspose.Tasks](../../extendedattributedefinition/)
* montage [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->