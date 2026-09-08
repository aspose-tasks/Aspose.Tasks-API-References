---
title: "ExtendedAttributeDefinition.RemoveLookupValue"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ExtendedAttributeDefinition-methode. Verwijdert een waarde uit de interne opzoeklijst. Dit is een voorkeursmethode voor manipulaties met de ValueList."
type: docs
weight: 340
url: /nl/net/aspose.tasks/extendedattributedefinition/removelookupvalue/
---
## ExtendedAttributeDefinition.RemoveLookupValue method

Verwijdert een waarde uit de interne opzoeklijst. Dit is een voorkeursmethode voor manipulaties met de [`ValueList`](../valuelist/).

```csharp
public void RemoveLookupValue(Value value)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | Waarde | Waarde die uit de opzoeklijst moet worden verwijderd. |

## Opmerkingen

Deze methode werkt alleen voor [`ExtendedAttributeDefinition`](../) instanties waarvan [`CalculationType`](../calculationtype/) gelijk is aan Lookup.

## Voorbeelden

Toont hoe u uitgebreide attributen met zoekopdrachten kunt toevoegen voor toewijzingen.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Wijs resource "1 TRG: Trade Group" toe aan "TASK 1" door een ResourceAssignment-object te maken.
var resource = project.Resources.GetById(1);
var task = project.RootTask.Children.GetById(1);
var assignment = project.ResourceAssignments.Add(task, resource);

// Maak een aangepaste attribuutdefinitie met zoekopdracht.
var resExtendedAttributeDefinition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(
    CustomFieldType.Cost,
    ExtendedAttributeResource.Cost5,
    "My lookup resource cost");
project.ExtendedAttributes.Add(resExtendedAttributeDefinition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
resExtendedAttributeDefinition.AddLookupValue(firstValue);
resExtendedAttributeDefinition.AddLookupValue(secondValue);

// Deze waarde is te zien in de weergave "Resource usage" van MS Project.
var attributeValue = resExtendedAttributeDefinition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

// Maak een aangepaste attribuutdefinitie met zoekopdracht.
var taskCostAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost4, "My lookup task cost");
project.ExtendedAttributes.Add(taskCostAttr);
var taskFirstValue = new Value { NumericValue = 18, Description = "Task val 1", Id = 3, Val = "18" };
var resSecondValue = new Value { NumericValue = 30, Description = "Task val 2", Id = 4 };
var taskWrongValue = new Value { NumericValue = 99, Description = "Task val Wrong", Id = 5, Val = "18" };

taskCostAttr.AddLookupValue(taskFirstValue);
resExtendedAttributeDefinition.AddLookupValue(resSecondValue);

// Deze waarde is te zien in de weergave "Task usage" van MS Project.
assignment.ExtendedAttributes.Add(taskCostAttr.CreateExtendedAttribute(taskFirstValue));

// verkeerde waarden kunnen later worden verwijderd
taskCostAttr.RemoveLookupValue(taskWrongValue);

// werken met project...
```

### Zie ook

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


