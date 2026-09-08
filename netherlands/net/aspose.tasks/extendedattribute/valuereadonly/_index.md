---
title: "ExtendedAttribute.ValueReadOnly"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ExtendedAttribute-eigenschap. Haalt een waarde op die aangeeft of een waarde van deze ExtendedAttribute‑instantie alleen-lezen is. Retourneert true als een formule of rollup is gedefinieerd in de ExtendedAttributeDefinition voor dit object."
type: docs
weight: 100
url: /nl/net/aspose.tasks/extendedattribute/valuereadonly/
---
## ExtendedAttribute.ValueReadOnly property

Haalt een waarde op die aangeeft of een waarde van deze [`ExtendedAttribute`](../)‑instantie alleen-lezen is. Retourneert true als een formule of rollup is gedefinieerd in de [`ExtendedAttributeDefinition`](../../extendedattributedefinition/) voor dit object.

```csharp
public bool ValueReadOnly { get; }
```

## Voorbeelden

Toont hoe een aangepast veld toe te voegen waarvan de waarde wordt berekend met een formule die door de gebruiker is opgegeven.

```csharp
var project = new Project();

// maak een nieuwe taak uitgebreide attribuutdefinitie
var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, "Cost ratio");

// Voeg een formule toe aan het attribuut.
attribute.Formula = "[Cost] / [Actual Cost]";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// Maak een uitgebreid attribuut.
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

// We stellen de Formule in voor het uitgebreide attribuut, zodat het alleen-lezen is (de waarde wordt berekend met een formule).
// Uitvoer is "Value is read only"
Console.WriteLine(extendedAttribute.ValueReadOnly ? "Value is read only" : "Value is not read only");

// U kunt proberen de waarde van een alleen-lezen veld in te stellen, maar dit zal geen effect hebben.
extendedAttribute.NumericValue = -1000000M;

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost),
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());

task.Set(Tsk.Cost, 100m);
task.Set(Tsk.ActualCost, 120m);

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost), 
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());
```

### Zie ook

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


