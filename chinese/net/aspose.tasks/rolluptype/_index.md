---
title: "枚举 RollupType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.RollupType 枚举。指定汇总类型"
type: docs
weight: 1950
url: /zh/net/aspose.tasks/rolluptype/
---
## RollupType enumeration

指定汇总类型。

```csharp
public enum RollupType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Null | `0` | 指示空汇总类型。 |
| Maximum | `1` | 指示最大汇总类型。 |
| Minimum | `2` | 指示最小汇总类型。 |
| Count | `3` | 指示计数汇总类型。 |
| Sum | `4` | 指示求和汇总类型。 |
| Average | `5` | 指示平均汇总类型。 |
| AverageFirstSublevel | `6` | 指示第一子级平均汇总类型。 |
| CountFirstSublevel | `7` | 指示第一子级计数汇总类型。 |
| CountNonsummaries | `8` | 指示非汇总计数汇总类型。 |

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


