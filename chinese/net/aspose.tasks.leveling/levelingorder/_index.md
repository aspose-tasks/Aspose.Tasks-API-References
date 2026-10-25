---
title: "枚举 LevelingOrder"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Leveling.LevelingOrder 枚举。定义平衡顺序的可能取值"
type: docs
weight: 950
url: /zh/net/aspose.tasks.leveling/levelingorder/
---
## LevelingOrder enumeration

定义平衡顺序的可能取值。

```csharp
public enum LevelingOrder
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Standard | `1` | 考虑以下属性：前置关系、总余量（总余量更大的任务优先延迟）、开始日期、优先级。这是默认值。 |
| IdOnly | `2` | 任务按 Id 升序延迟。 |
| PriorityThenStandard | `3` | 首先考虑优先级，然后与 Standard 相同的属性。 |

### 另见

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


