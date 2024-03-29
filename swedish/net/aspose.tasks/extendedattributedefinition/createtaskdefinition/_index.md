---
title: ExtendedAttributeDefinition.CreateTaskDefinition
second_title: Aspose.Tasks för .NET API-referens
description: ExtendedAttributeDefinition metod. Fabriksmetod som skapar en enkel utökad attributdefinition som Microsoft Project visar som Ingen. Den harCalculationType är lika medNone och kan endast användas i Tasks. Du måste specificeracustomFieldType fieldId ochalias när du anropar den här metoden.
type: docs
weight: 40
url: /sv/net/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---
## CreateTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createtaskdefinition}

Fabriksmetod som skapar en enkel utökad attributdefinition, som Microsoft Project visar som "Ingen". Den har[`CalculationType`](../calculationtype/) är lika medNone och kan endast användas i Tasks. Du måste specificera*customFieldType* ,*fieldId* och*alias* när du anropar den här metoden.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeTask fieldId, string alias)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| customFieldType | CustomFieldType | Den angivna[`CustomFieldType`](../../customfieldtype/) typ. |
| fieldId | ExtendedAttributeTask | Den angivna[`ExtendedAttributeTask`](../../extendedattributetask/) fält-ID. |
| alias | String | Den angivnaString alias. |

### Returvärde

Skapade instans av[`ExtendedAttributeDefinition`](../) klass med specificerad*customFieldType* ,*fieldId* och*alias*.

### Exempel

Använd det här exemplet för att skapa en anpassad textfältsdefinition:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

### Se även

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namnutrymme [Aspose.Tasks](../../extendedattributedefinition/)
* hopsättning [Aspose.Tasks](../../../)

---

## CreateTaskDefinition(ExtendedAttributeTask, string) {#createtaskdefinition_1}

Fabriksmetod som skapar en enkel utökad attributdefinition, som Microsoft Project visar som "Ingen". Den har[`CalculationType`](../calculationtype/) är lika medNone och kan endast användas i Tasks. Du måste specificera*fieldId* och*alias* när den här metoden anropas. Fälttypen härleds från fält-id.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | Den angivna[`ExtendedAttributeTask`](../../extendedattributetask/) fält-ID. |
| alias | String | Den angivnaString alias. |

### Returvärde

Skapade instans av[`ExtendedAttributeDefinition`](../) klass med specificerad*fieldId* och*alias*.

### Exempel

Använd det här exemplet för att skapa en anpassad textfältsdefinition:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

### Se även

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namnutrymme [Aspose.Tasks](../../extendedattributedefinition/)
* hopsättning [Aspose.Tasks](../../../)


