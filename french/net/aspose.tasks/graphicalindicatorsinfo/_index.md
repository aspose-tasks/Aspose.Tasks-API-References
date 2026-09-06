---
title: "Classe GraphicalIndicatorsInfo"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.GraphicalIndicatorsInfo. Représente une définition d'indicateurs graphiques associée à un attribut étendu"
type: docs
weight: 760
url: /fr/net/aspose.tasks/graphicalindicatorsinfo/
---
## GraphicalIndicatorsInfo class

Représente une définition d'indicateurs graphiques associée à un attribut étendu.

```csharp
public sealed class GraphicalIndicatorsInfo
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [GraphicalIndicatorsInfo](graphicalindicatorsinfo/)() | Initialise une nouvelle instance du type `GraphicalIndicatorsInfo`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Criteria](../../aspose.tasks/graphicalindicatorsinfo/criteria/) { get; } | Obtient une liste de critères d'indicateur graphique. |
| [ProjectSummaryInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/projectsummaryinheritfromnonsummaryrows/) { get; set; } | Obtient ou définit le drapeau indiquant si la ligne de résumé du projet hérite des critères des lignes de résumé. |
| [ShowDataValuesInTooltip](../../aspose.tasks/graphicalindicatorsinfo/showdatavaluesintooltip/) { get; set; } | Obtient ou définit le drapeau indiquant si les valeurs de données pour le champ doivent être affichées dans les infobulles. |
| [SummaryRowsInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/summaryrowsinheritfromnonsummaryrows/) { get; set; } | Obtient ou définit le drapeau indiquant si les lignes de résumé héritent des critères des lignes non résumées. |

## Exemples

Montre comment configurer un indicateur graphique pour un attribut étendu.

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

// Le critère 'IsWithin' nécessite 2 valeurs.
GraphicalIndicatorCriteria criteria2 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsWithin,
    4,
    new GraphicalIndicatorCriteriaValue(101),
    new GraphicalIndicatorCriteriaValue(1000m));

// Le critère 'IsAnyValue' ne nécessite pas de valeurs.
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

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


