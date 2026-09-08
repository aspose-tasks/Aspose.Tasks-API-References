---
title: "Enum GraphicalIndicatorCriteriaType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.GraphicalIndicatorCriteriaType‑enum. Vertegenwoordigt de plaatsing van grafische indicatorcriteria"
type: docs
weight: 740
url: /nl/net/aspose.tasks/graphicalindicatorcriteriatype/
---
## GraphicalIndicatorCriteriaType enumeration

Stelt de plaatsing van grafische indicatorcriteria voor.

```csharp
public enum GraphicalIndicatorCriteriaType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| NonSummaryRows | `0` | Vertegenwoordigt niet‑samenvattingsrijen. |
| SummaryRows | `1` | Vertegenwoordigt samenvattingsrijen. |
| ProjectSummary | `2` | Vertegenwoordigt de project‑samenvattingstaakrij. |

## Voorbeelden

Toont hoe een grafische indicator in te stellen voor een uitgebreid attribuut.

```csharp
Project project = new Project();

var def = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, "Number field");
project.ExtendedAttributes.Add(def);
def.GraphicalIndicator = new GraphicalIndicatorsInfo();

GraphicalIndicatorCriteria criteria1 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsLessThan,
    2,
    new GraphicalIndicatorCriteriaValue(100m));

// 'IsWithin'-criteria vereist 2 waarden.
GraphicalIndicatorCriteria criteria2 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsWithin,
    4,
    new GraphicalIndicatorCriteriaValue(101),
    new GraphicalIndicatorCriteriaValue(1000m));

// 'IsAnyValue'-criteria vereist geen waarden.
GraphicalIndicatorCriteria criteria3 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsAnyValue,
    4,
    null);

def.GraphicalIndicator.Criteria.Add(criteria1);
def.GraphicalIndicator.Criteria.Add(criteria2);
def.GraphicalIndicator.Criteria.Add(criteria3);

def.GraphicalIndicator.ProjectSummaryInheritFromNonSummaryRows = true;
def.GraphicalIndicator.SummaryRowsInheritFromNonSummaryRows = true;
def.GraphicalIndicator.ShowDataValuesInTooltip = false;

project.Save(OutDir + "CreateGraphicalIndicators_out.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


