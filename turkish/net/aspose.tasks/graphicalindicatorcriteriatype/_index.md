---
title: "Enum GraphicalIndicatorCriteriaType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.GraphicalIndicatorCriteriaType enum'ı. Grafik gösterge kriterlerinin yerleşimini temsil eder"
type: docs
weight: 740
url: /tr/net/aspose.tasks/graphicalindicatorcriteriatype/
---
## GraphicalIndicatorCriteriaType enumeration

Grafik gösterge kriterlerinin yerleşimini temsil eder.

```csharp
public enum GraphicalIndicatorCriteriaType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| NonSummaryRows | `0` | Özet olmayan satırları temsil eder. |
| SummaryRows | `1` | Özet satırlarını temsil eder. |
| ProjectSummary | `2` | Proje özet görev satırını temsil eder. |

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


