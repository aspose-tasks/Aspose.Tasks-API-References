---
title: "Klasse GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.GraphicalIndicatorCriteria klasse. Vertegenwoordigt één grafische indicatorcriterium dat is gekoppeld aan een uitgebreid attribuut"
type: docs
weight: 730
url: /nl/net/aspose.tasks/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria class

Stelt één criterium voor grafische indicatoren voor dat is gekoppeld aan een uitgebreid attribuut.

```csharp
public sealed class GraphicalIndicatorCriteria
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) | Initialiseert een nieuw exemplaar van het type `GraphicalIndicatorCriteria`. |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor_1)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) | Initialiseert een nieuw exemplaar van het type `GraphicalIndicatorCriteria`. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [ImageIndex](../../aspose.tasks/graphicalindicatorcriteria/imageindex/) { get; } | Haalt de index op van de afbeelding die moet worden weergegeven wanneer het veld aan de criteria voldoet. |
| [RowType](../../aspose.tasks/graphicalindicatorcriteria/rowtype/) { get; } | Haalt de waarde op van de enum [`GraphicalIndicatorCriteriaType`](../graphicalindicatorcriteriatype/) die aangeeft op welke rijen de indicator wordt toegepast. |
| [Test](../../aspose.tasks/graphicalindicatorcriteria/test/) { get; } | Haalt het type vergelijking op dat wordt gemaakt tussen de waarde van een uitgebreid attribuut en waarden die als criterium dienen voor de toepassing van de grafische indicator. [`FilterComparisonType`](../filtercomparisontype/) |
| [Value1](../../aspose.tasks/graphicalindicatorcriteria/value1/) { get; } | Haalt de waarde op die wordt gebruikt om de waarde van het uitgebreide attribuut te testen. |
| [Value2](../../aspose.tasks/graphicalindicatorcriteria/value2/) { get; } | Haalt de tweede waarde op die wordt gebruikt om de waarde van het uitgebreide attribuut te testen in het geval van de vergelijkingssoorten 'IsWithin' en 'IsNotWithin'. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [ToString](../../aspose.tasks/graphicalindicatorcriteria/tostring/)() | Retourneert de tekenreeksrepresentatie van de instantie van de `GraphicalIndicatorCriteria`-klasse. |

## Voorbeelden

Toont hoe grafische indicatorinformatie op te halen.

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


