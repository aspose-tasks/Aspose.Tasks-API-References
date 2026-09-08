---
title: "Klasse GraphicalIndicatorsInfo"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.GraphicalIndicatorsInfo class. Vertegenwoordigt een grafische indicatordefinitie die is gekoppeld aan een uitgebreid attribuut"
type: docs
weight: 760
url: /nl/net/aspose.tasks/graphicalindicatorsinfo/
---
## GraphicalIndicatorsInfo class

Stelt een definitie van grafische indicatoren voor die is gekoppeld aan een uitgebreid attribuut.

```csharp
public sealed class GraphicalIndicatorsInfo
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [GraphicalIndicatorsInfo](graphicalindicatorsinfo/)() | Initialiseert een nieuw exemplaar van het type `GraphicalIndicatorsInfo`. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Criteria](../../aspose.tasks/graphicalindicatorsinfo/criteria/) { get; } | Haalt een lijst met grafische indicatorcriteria op. |
| [ProjectSummaryInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/projectsummaryinheritfromnonsummaryrows/) { get; set; } | Haalt op of stelt de vlag in die aangeeft of de project‑samenvattingsrij criteria erft van samenvattingsrijen. |
| [ShowDataValuesInTooltip](../../aspose.tasks/graphicalindicatorsinfo/showdatavaluesintooltip/) { get; set; } | Haalt op of stelt de vlag in die aangeeft of gegevenswaarden voor het veld moeten worden weergegeven in tooltips. |
| [SummaryRowsInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/summaryrowsinheritfromnonsummaryrows/) { get; set; } | Haalt op of stelt de vlag in die aangeeft of samenvattingsrijen criteria erven van niet‑samenvattingsrijen. |

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


