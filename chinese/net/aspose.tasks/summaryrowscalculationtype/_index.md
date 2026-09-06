---
title: "枚举 SummaryRowsCalculationType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.SummaryRowsCalculationType 枚举。指定汇总行自定义属性值的计算类型。"
type: docs
weight: 2310
url: /zh/net/aspose.tasks/summaryrowscalculationtype/
---
## SummaryRowsCalculationType enumeration

指定汇总行自定义属性值计算的类型。

```csharp
public enum SummaryRowsCalculationType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| None | `0` | 表示汇总行的自定义属性值未计算。 |
| Rollup | `1` | 表示汇总行的自定义属性值使用在 [`RollupType`](../extendedattributedefinition/rolluptype/) 中定义的汇总函数进行计算。 |
| UseFormula | `2` | 表示汇总行的自定义属性值使用在 [`Formula`](../extendedattributedefinition/formula/) 中定义的公式进行计算。 |

## 示例

展示如何使用扩展属性定义的计算类型。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 16, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// 创建属性定义，类型为“Formula”，其中叶任务和汇总任务的值使用公式计算。
var calculation = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date5, null);
calculation.CalculationType = CalculationType.Formula;
calculation.SummaryRowsCalculationType = SummaryRowsCalculationType.UseFormula;
calculation.Formula = "[stARt]";
project.ExtendedAttributes.Add(calculation);

// 创建属性定义，其中汇总任务的值使用“Average”汇总类型计算。
var lookup = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, null);
lookup.SummaryRowsCalculationType = SummaryRowsCalculationType.Rollup;
lookup.RollupType = RollupType.Average;
project.ExtendedAttributes.Add(lookup);
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


