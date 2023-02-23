---
title: Enum ConstraintType
second_title: Aspose.Tasks for .NET API 参考
description: Aspose.Tasks.ConstraintType 枚举. 指定对任务的开始或完成日期的约束
type: docs
weight: 330
url: /zh/net/aspose.tasks/constrainttype/
---
## ConstraintType enumeration

指定对任务的开始或完成日期的约束。

```csharp
public enum ConstraintType
```

### 价值观

| 姓名 | 价值 | 描述 |
| --- | --- | --- |
| Undefined | `-1` | 该值未在原始项目文件中定义。 |
| AsSoonAsPossible | `0` | [`Start`](../tsk/start/)和[`Finish`](../tsk/finish/)的日期[`Task`](../task/)相对于父级安排 ASAP [`Start`](../tsk/start/)和[`Finish`](../tsk/finish/)日期和考虑[`TaskLinks`](../project/tasklinks/). |
| AsLateAsPossible | `1` | [`Start`](../tsk/start/)和[`Finish`](../tsk/finish/)的日期[`Task`](../task/)相对于父级安排 ALAP [`Start`](../tsk/start/)和[`Finish`](../tsk/finish/)日期和考虑[`TaskLinks`](../project/tasklinks/). |
| MustStartOn | `2` | 必须开始于 |
| MustFinishOn | `3` | 必须在 完成 |
| StartNoEarlierThan | `4` | 开始时间不早于 |
| StartNoLaterThan | `5` | 开始时间不晚于 |
| FinishNoEarlierThan | `6` | 不早于 完成 |
| FinishNoLaterThan | `7` | 完成时间不晚于 |

### 评论

导出到 XML 时，未定义的值将从生成的 XML 中消除。

### 也可以看看

* 命名空间 [Aspose.Tasks](../../aspose.tasks/)
* 部件 [Aspose.Tasks](../../)


