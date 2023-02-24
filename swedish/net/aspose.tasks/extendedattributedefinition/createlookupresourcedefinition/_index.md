---
title: ExtendedAttributeDefinition.CreateLookupResourceDefinition
second_title: Aspose.Tasks för .NET API-referens
description: ExtendedAttributeDefinition metod. Fabriksmetod som skapar en utökad attributdefinition med lookup. Den harCalculationType är lika medLookup och kan endast användas i Resurser. Du måste angefieldId ochalias när anropa denna metod. Fälttypen härleds från fältid.
type: docs
weight: 10
url: /sv/net/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---
## CreateLookupResourceDefinition(ExtendedAttributeResource, string) {#createlookupresourcedefinition_1}

Fabriksmetod som skapar en utökad attributdefinition med lookup. Den har[`CalculationType`](../calculationtype/) är lika medLookup och kan endast användas i Resurser. Du måste ange*fieldId* och*alias* när anropa denna metod. Fälttypen härleds från fält-id.

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | Den angivna[`ExtendedAttributeResource`](../../extendedattributeresource/) fält-ID. |
| alias | String | Den angivnaString alias. |

### Returvärde

Skapade instans av[`ExtendedAttributeDefinition`](../) klass med specificerad*fieldId* och*alias*.

### Exempel

Använd det här exemplet för att skapa en anpassad fältdefinition för en resurs med uppslag och fyll den sedan med textvärden:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Se även

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namnutrymme [Aspose.Tasks](../../extendedattributedefinition/)
* hopsättning [Aspose.Tasks](../../../)

---

## CreateLookupResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createlookupresourcedefinition}

Fabriksmetod som skapar en utökad attributdefinition med lookup. Den har[`CalculationType`](../calculationtype/) är lika medLookup och kan endast användas i Resurser. Du måste ange*customFieldType* ,*fieldId* och*alias* när anropa den här metoden.

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    CustomFieldType customFieldType, ExtendedAttributeResource fieldId, string alias)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| customFieldType | CustomFieldType | Den angivna[`CustomFieldType`](../../customfieldtype/) typ. |
| fieldId | ExtendedAttributeResource | Den angivna[`ExtendedAttributeResource`](../../extendedattributeresource/) fält-ID. |
| alias | String | Den angivnaString alias. |

### Returvärde

Skapade instans av[`ExtendedAttributeDefinition`](../) klass med specificerad*customFieldType* ,*fieldId* och*alias*.

### Exempel

Använd det här exemplet för att skapa en anpassad fältdefinition för en resurs med uppslag och fyll den sedan med textvärden:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Se även

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namnutrymme [Aspose.Tasks](../../extendedattributedefinition/)
* hopsättning [Aspose.Tasks](../../../)


