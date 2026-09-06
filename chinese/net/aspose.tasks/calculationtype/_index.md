---
title: "枚举 CalculationType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.CalculationType 枚举。指定自定义属性值的计算类型"
type: docs
weight: 220
url: /zh/net/aspose.tasks/calculationtype/
---
## CalculationType enumeration

指定自定义属性值计算的类型。

```csharp
public enum CalculationType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| None | `0` | 表示扩展属性没有公式查找表，仅存储用户设置的值。 |
| Lookup | `1` | 表示扩展属性的值受限于查找表中的值。 |
| Formula | `2` | 表示扩展属性的值使用在[`Formula`](../extendedattributedefinition/formula/)中定义的公式进行计算。 |

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


