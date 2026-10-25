---
title: "ExtendedAttribute.DateValue"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ExtendedAttribute-eigenschap. Haalt een waarde op of stelt deze in voor attributen met datumtypen Date Start Finish."
type: docs
weight: 20
url: /nl/net/aspose.tasks/extendedattribute/datevalue/
---
## ExtendedAttribute.DateValue property

Haalt op of stelt een waarde in voor attributen met datumtypen (Date, Start, Finish).

```csharp
public DateTime DateValue { get; set; }
```

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| InvalidOperationException | Wordt gegooid als de [`AttributeDefinition`](../attributedefinition/)‑eigenschap niet is geïnitialiseerd of het huidige attribuut geen datumattribuut is. |

## Voorbeelden

Toont hoe de attribuutdefinitie van het uitgebreide attribuut kan worden gewijzigd.

```csharp
var project = new Project();

// maak een nieuwe taak uitgebreide attribuutdefinitie
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, string.Empty);

// voeg een formule toe aan het attribuut.
definition.Alias = "Difference between Cost and Actual Cost";
definition.Formula = "[Cost]-[Actual Cost]";

project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));
task.Set(Tsk.Deadline, new DateTime(2020, 4, 22, 17, 0, 0));
task.Set(Tsk.Cost, 20);
task.Set(Tsk.ActualCost, 13);

// maak een uitgebreid attribuut
var extendedAttribute = definition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

Console.WriteLine("Before change:");
Console.WriteLine("Alias: " + definition.Alias);
Console.WriteLine("Field Id: " + extendedAttribute.FieldId);
Console.WriteLine("Value: " + extendedAttribute.NumericValue);

// maak een nieuwe datum‑uitgebreid‑attribuutdefinitie
var newDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Date, ExtendedAttributeTask.Date1, string.Empty);

// voeg een formule toe aan het attribuut.
newDefinition.Alias = "Days from finish to deadline";
newDefinition.Formula = "[Deadline] - [Finish]";
project.ExtendedAttributes.Add(newDefinition);

extendedAttribute = newDefinition.CreateExtendedAttribute();

Console.WriteLine();
Console.WriteLine("After change:");
Console.WriteLine("Alias: " + definition.Alias);
Console.WriteLine("Field Id: " + extendedAttribute.FieldId);
Console.WriteLine("Value: " + extendedAttribute.DateValue.Day);
```

### Zie ook

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


