---
title: "枚举 TaskStatus"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.TaskStatus 枚举。指定任务的状态"
type: docs
weight: 2460
url: /zh/net/aspose.tasks/taskstatus/
---
## TaskStatus enumeration

指定任务的状态。

```csharp
public enum TaskStatus
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Undefined | `-1` | 未定义的任务状态。 |
| Complete | `0` | 任务已完成 100%。 |
| OnSchedule | `1` | 如果分阶段累计完成百分比至少延伸到状态日期前一天，任务即按计划进行。 |
| Late | `2` | 如果分阶段累计完成百分比未在状态日期前一天的午夜达到，则任务延迟。 |
| Future | `3` | 当任务开始日期大于状态日期时，任务状态设置为“Future”。 |

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


