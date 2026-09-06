---
title: "Enumération GraphicalIndicatorCriteriaType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Enumération Aspose.Tasks.GraphicalIndicatorCriteriaType. Représente le placement des critères d'indicateur graphique"
type: docs
weight: 740
url: /fr/net/aspose.tasks/graphicalindicatorcriteriatype/
---
## GraphicalIndicatorCriteriaType enumeration

Représente le placement des critères d'indicateur graphique.

```csharp
public enum GraphicalIndicatorCriteriaType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| NonSummaryRows | `0` | Représente les lignes non récapitulatives. |
| SummaryRows | `1` | Représente les lignes récapitulatives. |
| ProjectSummary | `2` | Représente la ligne de tâche récapitulative du projet. |

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


