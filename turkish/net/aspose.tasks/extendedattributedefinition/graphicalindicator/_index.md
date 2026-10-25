---
title: "ExtendedAttributeDefinition.GraphicalIndicator"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ExtendedAttributeDefinition özelliği. Genişletilmiş öznitelikle ilişkili grafik gösterge bilgilerini alır veya ayarlar. MPP formatı için geçerlidir."
type: docs
weight: 160
url: /tr/net/aspose.tasks/extendedattributedefinition/graphicalindicator/
---
## ExtendedAttributeDefinition.GraphicalIndicator property

Genişletilmiş öznitelikle ilişkili grafik gösterge bilgilerini alır veya ayarlar. MPP formatı için geçerlidir.

```csharp
public GraphicalIndicatorsInfo GraphicalIndicator { get; set; }
```

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

* class [GraphicalIndicatorsInfo](../../graphicalindicatorsinfo/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


