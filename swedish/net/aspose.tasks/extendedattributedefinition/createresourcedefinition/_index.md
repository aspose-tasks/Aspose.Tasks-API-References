---
title: ExtendedAttributeDefinition.CreateResourceDefinition
second_title: Aspose.Tasks för .NET API-referens
description: ExtendedAttributeDefinition metod. Fabriksmetod som skapar en enkel utökad attributdefinition som Microsoft Project visar som Ingen. Den harCalculationType är lika medNone och kan endast användas i Resource. Du måste angecustomFieldType fieldId ochalias när anropa den här metoden.
type: docs
weight: 30
url: /sv/net/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---
## CreateResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createresourcedefinition}

Fabriksmetod som skapar en enkel utökad attributdefinition, som Microsoft Project visar som "Ingen". Den har[`CalculationType`](../calculationtype/) är lika medNone och kan endast användas i Resource. Du måste ange*customFieldType* ,*fieldId* och*alias* när anropa den här metoden.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeResource fieldId, string alias)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| customFieldType | CustomFieldType | Den angivna[`CustomFieldType`](../../customfieldtype/) typ. |
| fieldId | ExtendedAttributeResource | Den angivna[`ExtendedAttributeResource`](../../extendedattributeresource/) fält-ID. |
| alias | String | Den angivnaString alias. |

### Returvärde

Skapade instans av[`ExtendedAttributeDefinition`](../) klass med specificerad*customFieldType* ,*fieldId* och*alias*.

### Exempel

Använd det här exemplet för att skapa en anpassad textfältsdefinition:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Se även

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namnutrymme [Aspose.Tasks](../../extendedattributedefinition/)
* hopsättning [Aspose.Tasks](../../../)

---

## CreateResourceDefinition(ExtendedAttributeResource, string) {#createresourcedefinition_1}

Fabriksmetod som skapar en enkel utökad attributdefinition, som Microsoft Project visar som "Ingen". Den har[`CalculationType`](../calculationtype/) är lika medNone och kan endast användas i Resource. Du måste ange*fieldId* och*alias* när anropa denna metod. Fälttypen härleds från fält-id.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | Den angivna[`ExtendedAttributeResource`](../../extendedattributeresource/) fält-ID. |
| alias | String | Den angivnaString alias. |

### Returvärde

Skapade instans av[`ExtendedAttributeDefinition`](../) klass med specificerad*fieldId* och*alias*.

### Exempel

Använd det här exemplet för att skapa en anpassad textfältsdefinition:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Se även

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namnutrymme [Aspose.Tasks](../../extendedattributedefinition/)
* hopsättning [Aspose.Tasks](../../../)


