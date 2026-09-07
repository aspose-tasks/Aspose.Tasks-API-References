---
title: "Enum GraphicalIndicatorCriteriaType"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "Aspose.Tasks.GraphicalIndicatorCriteriaType Enum. Stellt die Platzierung von grafischen Indikator‑Kriterien dar"
type: docs
weight: 740
url: /de/net/aspose.tasks/graphicalindicatorcriteriatype/
---
## GraphicalIndicatorCriteriaType enumeration

Stellt die Platzierung von grafischen Indikator‑Kriterien dar.

```csharp
public enum GraphicalIndicatorCriteriaType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| NonSummaryRows | `0` | Stellt Nicht‑Zusammenfassungszeilen dar. |
| SummaryRows | `1` | Stellt Zusammenfassungszeilen dar. |
| ProjectSummary | `2` | Stellt die Projekt‑Zusammenfassungs‑Aufgabenzeile dar. |

## Beispiele

Zeigt, wie man einen grafischen Indikator für ein erweitertes Attribut einrichtet.

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

// 'IsWithin'-Kriterium erfordert 2 Werte.
GraphicalIndicatorCriteria criteria2 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsWithin,
    4,
    new GraphicalIndicatorCriteriaValue(101),
    new GraphicalIndicatorCriteriaValue(1000m));

// 'IsAnyValue'-Kriterium erfordert keine Werte.
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

### Siehe auch

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


