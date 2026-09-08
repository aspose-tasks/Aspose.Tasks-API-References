---
title: "Klasse ExtendedAttribute"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.ExtendedAttribute class. Vertegenwoordigt uitgebreide attributen"
type: docs
weight: 520
url: /nl/net/aspose.tasks/extendedattribute/
---
## ExtendedAttribute class

Stelt uitgebreide attributen voor.

```csharp
public class ExtendedAttribute
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [AttributeDefinition](../../aspose.tasks/extendedattribute/attributedefinition/) { get; } | Haalt de attribuutdefinitie op. |
| [DateValue](../../aspose.tasks/extendedattribute/datevalue/) { get; set; } | Haalt op of stelt een waarde in voor attributen met datumtypen (Date, Start, Finish). |
| [DurationValue](../../aspose.tasks/extendedattribute/durationvalue/) { get; set; } | Haalt op of stelt een waarde in voor attributen met het type 'Duration'. |
| [FieldId](../../aspose.tasks/extendedattribute/fieldid/) { get; } | Haalt de id van een veld op. |
| [FlagValue](../../aspose.tasks/extendedattribute/flagvalue/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of een vlag is ingesteld voor een attribuut met het type 'Flag'. |
| [IsErrorValue](../../aspose.tasks/extendedattribute/iserrorvalue/) { get; } | Haalt op of de berekening van de waarde van het uitgebreide attribuut in een fout is geëindigd. |
| [NumericValue](../../aspose.tasks/extendedattribute/numericvalue/) { get; set; } | Haalt op of stelt een waarde in voor attributen met numerieke typen (Cost, Number). |
| [TextValue](../../aspose.tasks/extendedattribute/textvalue/) { get; set; } | Haalt op of stelt een waarde in voor attributen met het type 'Text'. |
| [ValueGuid](../../aspose.tasks/extendedattribute/valueguid/) { get; } | Haalt de guid van een opzoekwaarde op. |
| [ValueReadOnly](../../aspose.tasks/extendedattribute/valuereadonly/) { get; } | Haalt een waarde op die aangeeft of een waarde van deze `ExtendedAttribute`-instantie alleen-lezen is. Retourneert true als een formule of roll-up is gedefinieerd in de [`ExtendedAttributeDefinition`](../extendedattributedefinition/) voor dit object. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [ToString](../../aspose.tasks/extendedattribute/tostring/)() | Retourneert een korte tekenreeksrepresentatie van een uitgebreid attribuut. |

## Opmerkingen

Momenteel worden alle typen uitgebreide attributen ondersteund die worden gelezen uit MSP Xml 2003/2007 en mpp 2003. Voor MSP mpp 2007 worden alle uitgebreide attributen gelezen, behalve duur- en vlagtype.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


