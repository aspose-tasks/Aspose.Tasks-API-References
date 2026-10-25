---
title: "Enum SummaryRowsCalculationType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.SummaryRowsCalculationType enum. Specificeert het type berekening van de waarde van aangepaste attributen voor samenvattingsrijen."
type: docs
weight: 2310
url: /nl/net/aspose.tasks/summaryrowscalculationtype/
---
## SummaryRowsCalculationType enumeration

Specificeert het type van een berekening van de waarde van een aangepast attribuut voor samenvattingsrijen.

```csharp
public enum SummaryRowsCalculationType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| None | `0` | Betekent dat de waarde van het aangepaste attribuut voor samenvattingsrijen niet wordt berekend. |
| Rollup | `1` | Betekent dat de waarde van het aangepaste attribuut voor samenvattingsrijen wordt berekend met de roll‑up‑functie die is gedefinieerd in [`RollupType`](../extendedattributedefinition/rolluptype/). |
| UseFormula | `2` | Betekent dat de waarde van het aangepaste attribuut voor samenvattingsrijen wordt berekend met de formule die is gedefinieerd in [`Formula`](../extendedattributedefinition/formula/). |

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


