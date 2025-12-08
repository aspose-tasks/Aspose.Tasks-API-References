---
title: Enum TaskStatus
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.TaskStatus enum. Specifies the status of a task
type: docs
weight: 2410
url: /net/aspose.tasks/taskstatus/
---
## TaskStatus enumeration

Specifies the status of a task.

```csharp
public enum TaskStatus
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Undefined | `-1` | Undefined task status. |
| Complete | `0` | The task is 100 percent complete. |
| OnSchedule | `1` | The task is on schedule if timephased cumulative percent complete is spread to at least the day before the status date. |
| Late | `2` | The task is late if the timephased cumulative percent complete does not reach midnight on the day before the status date. |
| Future | `3` | 'Future' task status is set when the task start date is greater than the status date. |

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


