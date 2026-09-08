---
title: "Klasse GlobalizationSettings"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.GlobalizationSettings klasse. Vertegenwoordigt de globalisatie-instellingen van het project"
type: docs
weight: 720
url: /nl/net/aspose.tasks/globalizationsettings/
---
## GlobalizationSettings class

Stelt de globalisatie-instellingen van het project voor.

```csharp
public class GlobalizationSettings
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [GlobalizationSettings](globalizationsettings/)() | De standaardconstructor. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| virtual [FalseLiteral](../../aspose.tasks/globalizationsettings/falseliteral/) { get; } | Haalt een tekenreeks op voor de booleaanse 'false'-literal die in een formule wordt gebruikt. |
| virtual [FormulaDateNA](../../aspose.tasks/globalizationsettings/formuladatena/) { get; } | Haalt de "NA" (lege waarde) literal op die in een formule voor een datumveld wordt gebruikt. |
| virtual [TrueLiteral](../../aspose.tasks/globalizationsettings/trueliteral/) { get; } | Haalt een tekenreeks op voor de booleaanse 'true'-literal die in een formule wordt gebruikt. |

## Opmerkingen

De aanbevolen manier is om door het hele project cultuuronafhankelijke literals of opmaak te gebruiken. Als een project echter cultuur‑specifieke literals gebruikt, kan deze klasse worden gebruikt om de formule‑berekeningsengine te helpen die literals te parseren.

## Voorbeelden

Toont hoe de taalspecifieke instellingen van het project worden ingesteld.

```csharp
var project = new Project();

var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, "Number");
attribute.Formula = "IIf(ProjDateValue('n.a.')=[Date1];100;200)";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// Maak een uitgebreid attribuut.
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

var attributeDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "Date");

task.ExtendedAttributes.Add(attributeDate.CreateExtendedAttribute(DateTime.MinValue));

Console.WriteLine(extendedAttribute.NumericValue);

project.GlobalizationSettings = new MyGlobalizationSettings();

Console.WriteLine(extendedAttribute.NumericValue);
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


