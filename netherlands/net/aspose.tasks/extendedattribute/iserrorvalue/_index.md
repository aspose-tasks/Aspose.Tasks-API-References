---
title: "ExtendedAttribute.IsErrorValue"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ExtendedAttribute property. Haalt op of de berekening van de waarde van uitgebreide attributen in een fout is geëindigd"
type: docs
weight: 60
url: /nl/net/aspose.tasks/extendedattribute/iserrorvalue/
---
## ExtendedAttribute.IsErrorValue property

Haalt op of de berekening van de waarde van het uitgebreide attribuut in een fout is geëindigd.

```csharp
public bool IsErrorValue { get; }
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


