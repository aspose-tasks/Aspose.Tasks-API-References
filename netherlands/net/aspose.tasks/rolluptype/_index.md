---
title: "Enum RollupType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.RollupType enum. Specificeert het rollup-type"
type: docs
weight: 1950
url: /nl/net/aspose.tasks/rolluptype/
---
## RollupType enumeration

Specificeert het roll-uptype.

```csharp
public enum RollupType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Null | `0` | Geeft Null rollup-type aan. |
| Maximum | `1` | Geeft Maximum rollup-type aan. |
| Minimum | `2` | Geeft Minimum rollup-type aan. |
| Count | `3` | Geeft Count rollup-type aan. |
| Sum | `4` | Geeft Sum rollup-type aan. |
| Average | `5` | Geeft Average rollup-type aan. |
| AverageFirstSublevel | `6` | Geeft Average First Sublevel rollup-type aan. |
| CountFirstSublevel | `7` | Geeft Count First Sublevel rollup-type aan. |
| CountNonsummaries | `8` | Geeft Count Non-Summaries rollup-type aan. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


