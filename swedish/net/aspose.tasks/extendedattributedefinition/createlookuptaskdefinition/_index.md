---
title: ExtendedAttributeDefinition.CreateLookupTaskDefinition
second_title: Aspose.Tasks för .NET API-referens
description: ExtendedAttributeDefinition metod. Fabriksmetod som skapar en utökad attributdefinition med lookup. Den harCalculationType är lika medLookup och kan endast användas i Tasks. Du måste specificerafieldId ochalias när anropa denna metod. Fälttypen härleds från fältid.
type: docs
weight: 20
url: /sv/net/aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/
---
## CreateLookupTaskDefinition(ExtendedAttributeTask, string) {#createlookuptaskdefinition_1}

Fabriksmetod som skapar en utökad attributdefinition med lookup. Den har[`CalculationType`](../calculationtype/) är lika medLookup och kan endast användas i Tasks. Du måste specificera*fieldId* och*alias* när anropa denna metod. Fälttypen härleds från fält-id.

```csharp
public static ExtendedAttributeDefinition CreateLookupTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | Den angivna[`ExtendedAttributeTask`](../../extendedattributetask/) fält-ID. |
| alias | String | Den angivnaString alias. |

### Returvärde

Skapade instans av[`ExtendedAttributeDefinition`](../) klass med specificerad*fieldId* och*alias*.

### Exempel

Använd det här exemplet för att skapa en anpassad fältdefinition för en uppgift med uppslag och fyll den sedan med textvärden:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
taskTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(taskTextAttr);
```

### Se även

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namnutrymme [Aspose.Tasks](../../extendedattributedefinition/)
* hopsättning [Aspose.Tasks](../../../)

---

## CreateLookupTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createlookuptaskdefinition}

Fabriksmetod som skapar en utökad attributdefinition med lookup. Den har[`CalculationType`](../calculationtype/) är lika medLookup och kan endast användas i Tasks. Du måste specificera*customFieldType* ,*fieldId* och*alias* när anropa den här metoden.

```csharp
public static ExtendedAttributeDefinition CreateLookupTaskDefinition(
    CustomFieldType customFieldType, ExtendedAttributeTask fieldId, string alias)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| customFieldType | CustomFieldType | Den angivna[`CustomFieldType`](../../customfieldtype/) typ. |
| fieldId | ExtendedAttributeTask | Den angivna[`ExtendedAttributeTask`](../../extendedattributetask/) fält-ID. |
| alias | String | Den angivnaString alias. |

### Returvärde

Skapade instans av[`ExtendedAttributeDefinition`](../) klass med specificerad*customFieldType* ,*fieldId* och*alias*.

### Exempel

Använd det här exemplet för att skapa en anpassad fältdefinition för en uppgift med uppslag och fyll den sedan med textvärden:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
taskTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(taskTextAttr);
```

### Se även

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namnutrymme [Aspose.Tasks](../../extendedattributedefinition/)
* hopsättning [Aspose.Tasks](../../../)


