---
title: "ExtendedAttributeDefinition.RollupType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ExtendedAttributeDefinition-eigenschap. Haalt of stelt de manier in waarop roll-ups worden berekend."
type: docs
weight: 230
url: /nl/net/aspose.tasks/extendedattributedefinition/rolluptype/
---
## ExtendedAttributeDefinition.RollupType property

Haalt de manier waarop roll-ups worden berekend op of stelt deze in.

```csharp
public RollupType RollupType { get; set; }
```

## Opmerkingen

Schrijven wordt momenteel alleen ondersteund voor het Xml-formaat.

## Voorbeelden

Toont hoe te werken met het berekeningstype van een uitgebreide attribuutdefinitie.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 16, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// maak een attribuutdefinitie met type 'Formula' waarbij waarden voor leaf-taken en samenvattingstaken worden berekend met een formule.
var calculation = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date5, null);
calculation.CalculationType = CalculationType.Formula;
calculation.SummaryRowsCalculationType = SummaryRowsCalculationType.UseFormula;
calculation.Formula = "[stARt]";
project.ExtendedAttributes.Add(calculation);

// maak een attribuutdefinitie waarbij waarden voor samenvattingstaken worden berekend met rollup-type 'Average'.
var lookup = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, null);
lookup.SummaryRowsCalculationType = SummaryRowsCalculationType.Rollup;
lookup.RollupType = RollupType.Average;
project.ExtendedAttributes.Add(lookup);
```

### Zie ook

* enum [RollupType](../../rolluptype/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


