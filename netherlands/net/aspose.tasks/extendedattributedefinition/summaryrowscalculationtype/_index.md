---
title: "ExtendedAttributeDefinition.SummaryRowsCalculationType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ExtendedAttributeDefinition-eigenschap. Haalt het type berekening op of stelt dit in voor de waarde van aangepaste attributen voor samenvattingsrijen"
type: docs
weight: 260
url: /nl/net/aspose.tasks/extendedattributedefinition/summaryrowscalculationtype/
---
## ExtendedAttributeDefinition.SummaryRowsCalculationType property

Haalt het type berekening van de waarde van het aangepaste attribuut voor samenvattingsrijen op of stelt dit in.

```csharp
public SummaryRowsCalculationType SummaryRowsCalculationType { get; set; }
```

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

* enum [SummaryRowsCalculationType](../../summaryrowscalculationtype/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


