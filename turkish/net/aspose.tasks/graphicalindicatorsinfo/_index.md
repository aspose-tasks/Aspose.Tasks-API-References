---
title: "GraphicalIndicatorsInfo sınıfı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.GraphicalIndicatorsInfo sınıfı. Genişletilmiş bir öznitelikle ilişkili bir grafik gösterge tanımını temsil eder"
type: docs
weight: 760
url: /tr/net/aspose.tasks/graphicalindicatorsinfo/
---
## GraphicalIndicatorsInfo class

Genişletilmiş bir öznitelikle ilişkili bir grafik gösterge tanımını temsil eder.

```csharp
public sealed class GraphicalIndicatorsInfo
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [GraphicalIndicatorsInfo](graphicalindicatorsinfo/)() | `GraphicalIndicatorsInfo` tipinin yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Criteria](../../aspose.tasks/graphicalindicatorsinfo/criteria/) { get; } | Grafik gösterge ölçütlerinin bir listesini alır. |
| [ProjectSummaryInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/projectsummaryinheritfromnonsummaryrows/) { get; set; } | Proje özet satırının ölçütleri özet satırlardan devralıp devralmadığını gösteren bayrağı alır veya ayarlar. |
| [ShowDataValuesInTooltip](../../aspose.tasks/graphicalindicatorsinfo/showdatavaluesintooltip/) { get; set; } | Alan için veri değerlerinin araç ipuçlarında gösterilip gösterilmeyeceğini belirten bayrağı alır veya ayarlar. |
| [SummaryRowsInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/summaryrowsinheritfromnonsummaryrows/) { get; set; } | Özet satırların ölçütleri özet olmayan satırlardan devralıp devralmadığını gösteren bayrağı alır veya ayarlar. |

## Örnekler

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


