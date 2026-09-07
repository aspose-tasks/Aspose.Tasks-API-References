---
title: "Klasse GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "Aspose.Tasks.GraphicalIndicatorCriteria Klasse. Stellt ein grafisches Indikator‑Kriterium dar, das einem erweiterten Attribut zugeordnet ist"
type: docs
weight: 730
url: /de/net/aspose.tasks/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria class

Stellt ein grafisches Indikator‑Kriterium dar, das einem erweiterten Attribut zugeordnet ist.

```csharp
public sealed class GraphicalIndicatorCriteria
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) | Initialisiert eine neue Instanz des Typs `GraphicalIndicatorCriteria`. |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor_1)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) | Initialisiert eine neue Instanz des Typs `GraphicalIndicatorCriteria`. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ImageIndex](../../aspose.tasks/graphicalindicatorcriteria/imageindex/) { get; } | Ruft den Index des Bildes ab, das angezeigt werden soll, wenn das Feld die Kriterien erfüllt. |
| [RowType](../../aspose.tasks/graphicalindicatorcriteria/rowtype/) { get; } | Ruft den Wert des `[`GraphicalIndicatorCriteriaType`](../graphicalindicatorcriteriatype/)` Enums ab, der angibt, für welche Zeilen der Indikator angewendet wird. |
| [Test](../../aspose.tasks/graphicalindicatorcriteria/test/) { get; } | Ruft den Vergleichstyp ab, der zwischen dem Wert des erweiterten Attributs und den Werten, die als Kriterium für die Anwendung des grafischen Indikators dienen, durchgeführt wird. `[`FilterComparisonType`](../filtercomparisontype/)` |
| [Value1](../../aspose.tasks/graphicalindicatorcriteria/value1/) { get; } | Ruft den Wert ab, der zum Testen des Wertes des erweiterten Attributs verwendet wird. |
| [Value2](../../aspose.tasks/graphicalindicatorcriteria/value2/) { get; } | Ruft den zweiten Wert ab, der zum Testen des Wertes des erweiterten Attributs im Fall der Vergleichstypen 'IsWithin' und 'IsNotWithin' verwendet wird. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [ToString](../../aspose.tasks/graphicalindicatorcriteria/tostring/)() | Gibt die Zeichenkettenrepräsentation der Instanz der Klasse `GraphicalIndicatorCriteria` zurück. |

## Beispiele

Zeigt, wie man Informationen zu grafischen Indikatoren abruft.

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


