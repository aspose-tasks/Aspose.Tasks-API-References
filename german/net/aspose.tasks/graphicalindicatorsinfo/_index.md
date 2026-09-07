---
title: "Klasse GraphicalIndicatorsInfo"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "Aspose.Tasks.GraphicalIndicatorsInfo Klasse. Stellt eine Definition von grafischen Indikatoren dar, die mit einem erweiterten Attribut verknüpft ist"
type: docs
weight: 760
url: /de/net/aspose.tasks/graphicalindicatorsinfo/
---
## GraphicalIndicatorsInfo class

Stellt eine Definition von grafischen Indikatoren dar, die mit einem erweiterten Attribut verknüpft ist.

```csharp
public sealed class GraphicalIndicatorsInfo
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [GraphicalIndicatorsInfo](graphicalindicatorsinfo/)() | Initialisiert eine neue Instanz des Typs `GraphicalIndicatorsInfo`. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Criteria](../../aspose.tasks/graphicalindicatorsinfo/criteria/) { get; } | Ruft eine Liste von grafischen Indikator‑Kriterien ab. |
| [ProjectSummaryInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/projectsummaryinheritfromnonsummaryrows/) { get; set; } | Ruft ab oder legt das Flag fest, das angibt, ob die Projekt‑Zusammenfassungszeile Kriterien von Zusammenfassungszeilen erbt. |
| [ShowDataValuesInTooltip](../../aspose.tasks/graphicalindicatorsinfo/showdatavaluesintooltip/) { get; set; } | Ruft ab oder legt das Flag fest, das angibt, ob Datenwerte für das Feld in Tooltips angezeigt werden sollen. |
| [SummaryRowsInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/summaryrowsinheritfromnonsummaryrows/) { get; set; } | Ruft ab oder legt das Flag fest, das angibt, ob Zusammenfassungszeilen Kriterien von Nicht‑Zusammenfassungszeilen erben. |

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


