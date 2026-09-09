---
title: "Sınıf GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.GraphicalIndicatorCriteria sınıfı. Genişletilmiş bir öznitelikle ilişkili bir grafik gösterge ölçütünü temsil eder"
type: docs
weight: 730
url: /tr/net/aspose.tasks/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria class

Genişletilmiş bir öznitelikle ilişkili bir grafik gösterge kriterini temsil eder.

```csharp
public sealed class GraphicalIndicatorCriteria
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) | `GraphicalIndicatorCriteria` tipinin yeni bir örneğini başlatır. |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor_1)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) | `GraphicalIndicatorCriteria` tipinin yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ImageIndex](../../aspose.tasks/graphicalindicatorcriteria/imageindex/) { get; } | Alan ölçütleri karşıladığında gösterilecek görüntünün dizinini alır. |
| [RowType](../../aspose.tasks/graphicalindicatorcriteria/rowtype/) { get; } | [`GraphicalIndicatorCriteriaType`](../graphicalindicatorcriteriatype/) enumunun değerini alır ve bu, göstergenin hangi satırlara uygulandığını belirtir. |
| [Test](../../aspose.tasks/graphicalindicatorcriteria/test/) { get; } | Genişletilmiş öznitelik değerleri ile grafik gösterge uygulaması için ölçüt olarak kullanılan değerler arasındaki karşılaştırma türünü alır. [`FilterComparisonType`](../filtercomparisontype/) |
| [Value1](../../aspose.tasks/graphicalindicatorcriteria/value1/) { get; } | Genişletilmiş özniteliğin değerini test etmek için kullanılan değeri alır. |
| [Value2](../../aspose.tasks/graphicalindicatorcriteria/value2/) { get; } | ‘IsWithin’ ve ‘IsNotWithin’ karşılaştırma türleri durumunda genişletilmiş özniteliğin değerini test etmek için kullanılan ikinci değeri alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [ToString](../../aspose.tasks/graphicalindicatorcriteria/tostring/)() | `GraphicalIndicatorCriteria` sınıfının örneğinin string temsilini döndürür. |

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


