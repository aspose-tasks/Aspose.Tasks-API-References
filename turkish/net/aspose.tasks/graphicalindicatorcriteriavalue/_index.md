---
title: "Sınıf GraphicalIndicatorCriteriaValue"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.GraphicalIndicatorCriteriaValue sınıfı. Grafik gösterge kriterlerinin koşul kontrolünde kullanılan bir değeri temsil eder."
type: docs
weight: 750
url: /tr/net/aspose.tasks/graphicalindicatorcriteriavalue/
---
## GraphicalIndicatorCriteriaValue class

Grafik göstergeler kriterinin koşul kontrolünde kullanılan bir değeri temsil eder.

```csharp
public sealed class GraphicalIndicatorCriteriaValue
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_1)(bool) | Sabit bayrak (bool) değeriyle GraphicalIndicatorCriteriaValue sınıfının bir örneğini oluşturur. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_2)(DateTime) | Sabit DateTime değeriyle GraphicalIndicatorCriteriaValue sınıfının bir örneğini oluşturur. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_3)(decimal) | Sabit decimal değeriyle GraphicalIndicatorCriteriaValue sınıfının bir örneğini oluşturur. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor)(Duration) | Sabit Duration değeriyle GraphicalIndicatorCriteriaValue sınıfının bir örneğini oluşturur. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_4)(string) | Sabit string değeriyle GraphicalIndicatorCriteriaValue sınıfının bir örneğini oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [IsFieldLink](../../aspose.tasks/graphicalindicatorcriteriavalue/isfieldlink/) { get; } | Mevcut örneğin bir alan bağlantısı (bir alanın değerini temsil eder) olup olmadığını alır. |
| [RawValue](../../aspose.tasks/graphicalindicatorcriteriavalue/rawvalue/) { get; } | Field değerinin temel sabitini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [CreateFieldLink](../../aspose.tasks/graphicalindicatorcriteriavalue/createfieldlink/)(Field) | Belirtilen MS Project alanının değerini temsil eden GraphicalIndicatorCriteriaValue sınıfının bir örneğini oluşturur. |
| override [ToString](../../aspose.tasks/graphicalindicatorcriteriavalue/tostring/)() | Geçerli nesneyi temsil eden bir dize döndürür. |

## Örnekler

Grafik göstergeleri bilgilerini nasıl alacağınızı gösterir.

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

Genişletilmiş bir öznitelik için grafik göstergeyi nasıl ayarlayacağınızı gösterir.

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

// ‘IsWithin’ kriteri 2 değer gerektirir.
GraphicalIndicatorCriteria criteria2 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsWithin,
    4,
    new GraphicalIndicatorCriteriaValue(101),
    new GraphicalIndicatorCriteriaValue(1000m));

// ‘IsAnyValue’ kriteri değer gerektirmez.
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

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


