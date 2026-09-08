---
title: "Klasse GraphicalIndicatorCriteriaValue"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.GraphicalIndicatorCriteriaValue klasse. Vertegenwoordigt een waarde die wordt gebruikt bij de voorwaardelijke controle van criteria voor grafische indicatoren"
type: docs
weight: 750
url: /nl/net/aspose.tasks/graphicalindicatorcriteriavalue/
---
## GraphicalIndicatorCriteriaValue class

Stelt een waarde voor die wordt gebruikt bij de voorwaardelijke controle van criteria voor grafische indicatoren.

```csharp
public sealed class GraphicalIndicatorCriteriaValue
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_1)(bool) | Maakt een instantie van de GraphicalIndicatorCriteriaValue klasse met een constante vlag (bool) waarde. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_2)(DateTime) | Maakt een instantie van de GraphicalIndicatorCriteriaValue klasse met een constante DateTime‑waarde. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_3)(decimal) | Maakt een instantie van de GraphicalIndicatorCriteriaValue klasse met een constante decimale waarde. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor)(Duration) | Maakt een instantie van de GraphicalIndicatorCriteriaValue klasse met een constante Duration‑waarde. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_4)(string) | Maakt een instantie van de GraphicalIndicatorCriteriaValue klasse met een constante string‑waarde. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [IsFieldLink](../../aspose.tasks/graphicalindicatorcriteriavalue/isfieldlink/) { get; } | Haalt op of de huidige instantie een veldkoppeling is (vertegenwoordigt een waarde van een veld). |
| [RawValue](../../aspose.tasks/graphicalindicatorcriteriavalue/rawvalue/) { get; } | Haalt de onderliggende constante van de veldwaarde op. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| static [CreateFieldLink](../../aspose.tasks/graphicalindicatorcriteriavalue/createfieldlink/)(Field) | Maakt een instantie van de GraphicalIndicatorCriteriaValue‑klasse die de waarde van het opgegeven MS Project‑veld vertegenwoordigt. |
| override [ToString](../../aspose.tasks/graphicalindicatorcriteriavalue/tostring/)() | Retourneert een string die het huidige object vertegenwoordigt. |

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


