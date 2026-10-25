---
title: "Classe GraphicalIndicatorCriteria"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.GraphicalIndicatorCriteria. Représente un critère d'indicateur graphique associé à un attribut étendu"
type: docs
weight: 730
url: /fr/net/aspose.tasks/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria class

Représente un critère d'indicateur graphique associé à un attribut étendu.

```csharp
public sealed class GraphicalIndicatorCriteria
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) | Initialise une nouvelle instance du type `GraphicalIndicatorCriteria`. |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor_1)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) | Initialise une nouvelle instance du type `GraphicalIndicatorCriteria`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [ImageIndex](../../aspose.tasks/graphicalindicatorcriteria/imageindex/) { get; } | Obtient l'index de l'image à afficher lorsque le champ répond aux critères. |
| [RowType](../../aspose.tasks/graphicalindicatorcriteria/rowtype/) { get; } | Obtient la valeur de l'énumération [`GraphicalIndicatorCriteriaType`](../graphicalindicatorcriteriatype/) qui indique pour quelles lignes l'indicateur est appliqué. |
| [Test](../../aspose.tasks/graphicalindicatorcriteria/test/) { get; } | Obtient le type de comparaison effectué entre la valeur de l'attribut étendu et les valeurs qui servent de critère pour l'application de l'indicateur graphique. [`FilterComparisonType`](../filtercomparisontype/) |
| [Value1](../../aspose.tasks/graphicalindicatorcriteria/value1/) { get; } | Obtient la valeur utilisée pour tester la valeur de l'attribut étendu. |
| [Value2](../../aspose.tasks/graphicalindicatorcriteria/value2/) { get; } | Obtient la deuxième valeur utilisée pour tester la valeur de l'attribut étendu dans le cas des types de comparaison 'IsWithin' et 'IsNotWithin'. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [ToString](../../aspose.tasks/graphicalindicatorcriteria/tostring/)() | Renvoie la représentation sous forme de chaîne de l'instance de la classe `GraphicalIndicatorCriteria`. |

## Exemples

Montre comment récupérer les informations des indicateurs graphiques.

```csharp
Project project = new Project(DataDir + "graphical_indicators.mpp");

foreach (var ea in project.ExtendedAttributes)
{
    if (ea.GraphicalIndicator == null)
    {
        continue;
    }

    Console.WriteLine("GI for field '{0}':", ea.FieldName);

    foreach (var criterion in ea.GraphicalIndicator.Criteria)
    {
        Console.WriteLine("Row type: {0}", criterion.RowType);
        Console.WriteLine("Image index: {0}", criterion.ImageIndex);
        Console.Write(criterion.Test);
        if (criterion.Value1 != null)
        {
            Console.Write(" ");
            Console.Write(criterion.Value1.RawValue);
        }

        if (criterion.Value2 != null)
        {
            Console.Write(" ");
            Console.WriteLine(criterion.Value2.RawValue);
        }

        Console.WriteLine();
    }
}
```

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


