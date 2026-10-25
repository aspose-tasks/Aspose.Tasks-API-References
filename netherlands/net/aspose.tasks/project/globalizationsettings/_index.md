---
title: "Project.GlobalizationSettings"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Projecteigenschap. Haalt de globalisatie‑taalspecifieke instellingen van het project op of stelt deze in"
type: docs
weight: 460
url: /nl/net/aspose.tasks/project/globalizationsettings/
---
## Project.GlobalizationSettings property

Haalt de globalisatie‑ (taalspecifieke) instellingen van het project op of stelt deze in.

```csharp
public GlobalizationSettings GlobalizationSettings { get; set; }
```

## Opmerkingen

De aanbevolen manier is om door het hele project cultuur‑invariante literals of opmaak te gebruiken. Als een project echter cultuur‑specifieke literals gebruikt, kan deze klasse worden gebruikt om de berekeningsengine te helpen die literals te parseren.

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

* class [GlobalizationSettings](../../globalizationsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


