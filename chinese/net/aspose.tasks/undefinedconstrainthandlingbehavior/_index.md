---
title: "枚举 UndefinedConstraintHandlingBehavior"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.UndefinedConstraintHandlingBehavior 枚举。指定用于处理具有未定义约束的任务的行为。"
type: docs
weight: 2630
url: /zh/net/aspose.tasks/undefinedconstrainthandlingbehavior/
---
## UndefinedConstraintHandlingBehavior enumeration

指定用于处理约束未定义任务的行为。

```csharp
public enum UndefinedConstraintHandlingBehavior
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| None | `0` | 从 XER 格式加载的默认行为。未采取任何操作。任务约束类型被设置为 'ConstraintType.Undefined'。 |
| SubstituteWithStartNoEarlierThan | `1` | 对于具有 'Undefined' 约束的任务，添加类型为 'ConstraintType.StartNoEarlierThan' 且日期 = Start 的约束。 |

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


