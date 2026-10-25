---
title: "类 GraphicalIndicatorsInfo"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.GraphicalIndicatorsInfo 类。表示与扩展属性关联的图形指示器定义"
type: docs
weight: 760
url: /zh/net/aspose.tasks/graphicalindicatorsinfo/
---
## GraphicalIndicatorsInfo class

表示与扩展属性关联的图形指示器定义。

```csharp
public sealed class GraphicalIndicatorsInfo
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [GraphicalIndicatorsInfo](graphicalindicatorsinfo/)() | 初始化 `GraphicalIndicatorsInfo` 类型的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Criteria](../../aspose.tasks/graphicalindicatorsinfo/criteria/) { get; } | 获取图形指示器标准的列表。 |
| [ProjectSummaryInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/projectsummaryinheritfromnonsummaryrows/) { get; set; } | 获取或设置标志，指示项目摘要行是否从摘要行继承标准。 |
| [ShowDataValuesInTooltip](../../aspose.tasks/graphicalindicatorsinfo/showdatavaluesintooltip/) { get; set; } | 获取或设置标志，指示该字段的数据值是否应在工具提示中显示。 |
| [SummaryRowsInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/summaryrowsinheritfromnonsummaryrows/) { get; set; } | 获取或设置标志，指示摘要行是否从非摘要行继承标准。 |

## 示例

展示如何为扩展属性设置图形指示器。

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

// 'IsWithin' 条件需要 2 个值。
GraphicalIndicatorCriteria criteria2 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsWithin,
    4,
    new GraphicalIndicatorCriteriaValue(101),
    new GraphicalIndicatorCriteriaValue(1000m));

// 'IsAnyValue' 条件不需要值。
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

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


