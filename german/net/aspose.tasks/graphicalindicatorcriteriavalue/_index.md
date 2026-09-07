---
title: "Klasse GraphicalIndicatorCriteriaValue"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "Aspose.Tasks.GraphicalIndicatorCriteriaValue Klasse. Stellt einen Wert dar, der bei der Bedingungsprüfung von Kriterien grafischer Indikatoren verwendet wird"
type: docs
weight: 750
url: /de/net/aspose.tasks/graphicalindicatorcriteriavalue/
---
## GraphicalIndicatorCriteriaValue class

Stellt einen Wert dar, der bei der Bedingungsprüfung von Kriterien grafischer Indikatoren verwendet wird.

```csharp
public sealed class GraphicalIndicatorCriteriaValue
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_1)(bool) | Erstellt eine Instanz der Klasse GraphicalIndicatorCriteriaValue mit einem konstanten Flag‑Wert (bool). |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_2)(DateTime) | Erstellt eine Instanz der Klasse GraphicalIndicatorCriteriaValue mit einem konstanten DateTime‑Wert. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_3)(decimal) | Erstellt eine Instanz der Klasse GraphicalIndicatorCriteriaValue mit einem konstanten Dezimalwert. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor)(Duration) | Erstellt eine Instanz der Klasse GraphicalIndicatorCriteriaValue mit einem konstanten Duration‑Wert. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_4)(string) | Erstellt eine Instanz der Klasse GraphicalIndicatorCriteriaValue mit einem konstanten Zeichenfolgenwert. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [IsFieldLink](../../aspose.tasks/graphicalindicatorcriteriavalue/isfieldlink/) { get; } | Ermittelt, ob die aktuelle Instanz ein Feldverweis ist (repräsentiert einen Wert eines Feldes). |
| [RawValue](../../aspose.tasks/graphicalindicatorcriteriavalue/rawvalue/) { get; } | Ermittelt die zugrunde liegende Konstante des Feldwerts. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [CreateFieldLink](../../aspose.tasks/graphicalindicatorcriteriavalue/createfieldlink/)(Field) | Erstellt eine Instanz der Klasse GraphicalIndicatorCriteriaValue, die den Wert des angegebenen MS Project‑Feldes darstellt. |
| override [ToString](../../aspose.tasks/graphicalindicatorcriteriavalue/tostring/)() | Gibt eine Zeichenfolge zurück, die das aktuelle Objekt darstellt. |

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


