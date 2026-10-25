---
title: "Enumeratie CalculationType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.CalculationType enum. Specificeert het type van een berekening van de waarde van aangepaste attributen"
type: docs
weight: 220
url: /nl/net/aspose.tasks/calculationtype/
---
## CalculationType enumeration

Specificeert het type van een berekening van de waarde van het aangepaste attribuut.

```csharp
public enum CalculationType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| None | `0` | Betekent dat het uitgebreide attribuut geen opzoektabel of formule heeft en eenvoudig de door de gebruiker ingestelde waarde opslaat. |
| Lookup | `1` | Betekent dat de waarde van het uitgebreide attribuut beperkt is tot waarden uit een opzoektabel. |
| Formula | `2` | Betekent dat de waarde van het uitgebreide attribuut wordt berekend met behulp van de formule die is gedefinieerd in [`Formula`](../extendedattributedefinition/formula/). |

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


