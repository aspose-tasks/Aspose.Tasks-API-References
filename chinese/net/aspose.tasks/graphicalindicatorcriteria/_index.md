---
title: "类 GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.GraphicalIndicatorCriteria 类。表示与扩展属性关联的一个图形指示器条件"
type: docs
weight: 730
url: /zh/net/aspose.tasks/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria class

表示与扩展属性关联的一个图形指示器条件。

```csharp
public sealed class GraphicalIndicatorCriteria
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) | 初始化 `GraphicalIndicatorCriteria` 类型的新实例。 |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor_1)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) | 初始化 `GraphicalIndicatorCriteria` 类型的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [ImageIndex](../../aspose.tasks/graphicalindicatorcriteria/imageindex/) { get; } | 获取当字段满足条件时要显示的图像索引。 |
| [RowType](../../aspose.tasks/graphicalindicatorcriteria/rowtype/) { get; } | 获取 [`GraphicalIndicatorCriteriaType`](../graphicalindicatorcriteriatype/) 枚举的值，该枚举指示指示器适用于哪些行。 |
| [Test](../../aspose.tasks/graphicalindicatorcriteria/test/) { get; } | 获取在扩展属性的值与作为图形指示器应用条件的值之间进行的比较类型。[`FilterComparisonType`](../filtercomparisontype/) |
| [Value1](../../aspose.tasks/graphicalindicatorcriteria/value1/) { get; } | 获取用于测试扩展属性值的值。 |
| [Value2](../../aspose.tasks/graphicalindicatorcriteria/value2/) { get; } | 获取在 'IsWithin' 和 'IsNotWithin' 比较类型情况下用于测试扩展属性值的第二个值。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [ToString](../../aspose.tasks/graphicalindicatorcriteria/tostring/)() | 返回 `GraphicalIndicatorCriteria` 类实例的字符串表示形式。 |

## 示例

展示如何检索图形指示器信息。

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


