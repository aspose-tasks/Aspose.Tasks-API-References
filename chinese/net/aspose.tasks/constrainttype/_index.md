---
title: "枚举 ConstraintType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.ConstraintType 枚举。指定任务开始或结束日期的约束"
type: docs
weight: 330
url: /zh/net/aspose.tasks/constrainttype/
---
## ConstraintType enumeration

指定任务开始或结束日期的约束。

```csharp
public enum ConstraintType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Undefined | `-1` | 该值未在原始项目文件中定义。 |
| AsSoonAsPossible | `0` | [`Start`](../tsk/start/) 和 [`Finish`](../tsk/finish/) 日期的 [`Task`](../task/) 将根据父级 [`Start`](../tsk/start/) 和 [`Finish`](../tsk/finish/) 日期尽快安排，并考虑 [`TaskLinks`](../project/tasklinks/)。 |
| AsLateAsPossible | `1` | [`Start`](../tsk/start/) 和 [`Finish`](../tsk/finish/) 日期的 [`Task`](../task/) 按照父级 [`Start`](../tsk/start/) 和 [`Finish`](../tsk/finish/) 日期尽可能晚（ALAP）安排，并考虑 [`TaskLinks`](../project/tasklinks/)。 |
| MustStartOn | `2` | 必须开始于 |
| MustFinishOn | `3` | 必须完成于 |
| StartNoEarlierThan | `4` | 开始不早于 |
| StartNoLaterThan | `5` | 开始不晚于 |
| FinishNoEarlierThan | `6` | 完成不早于 |
| FinishNoLaterThan | `7` | 完成不晚于 |

## 备注

在导出为 XML 时，未定义的值将从生成的 XML 中删除。

## 示例

显示如何为任务设置约束 &lt;see cref=\"Aspose.Tasks.ConstraintType\" /&gt; ConstraintType.AsSoonAsPossible 约束。

```csharp
var project = new Project(DataDir + "Constraints/ConstraintAsLateAsPossible.mpp");

// 为 Id 为 11 的任务设置 As Soon As Possible 约束
var task = project.RootTask.Children.GetById(11);
task.Set(Tsk.ConstraintType, ConstraintType.AsSoonAsPossible);

SaveOptions options = new PdfSaveOptions();
options.StartDate = project.Get(Prj.StartDate);
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "AsSoonAsPossible_out.pdf", options);
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


