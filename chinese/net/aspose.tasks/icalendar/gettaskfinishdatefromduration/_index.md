---
title: "ICalendar.GetTaskFinishDateFromDuration"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ICalendar 方法。根据任务的开始日期拆分部分和工作持续时间计算任务的完成日期和时间。"
type: docs
weight: 50
url: /zh/net/aspose.tasks/icalendar/gettaskfinishdatefromduration/
---
## ICalendar.GetTaskFinishDateFromDuration method

根据任务的开始日期、拆分部分和工作持续时间计算任务的完成日期和时间。

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 任务 | 任务 | 用于计算完成日期的任务。 |
| 持续时间 | TimeSpan | 要计算的持续时间。 |

### 返回值

给定开始日期和持续时间的任务完成日期。

## 备注

如果任务是汇总、为空或其开始日期未设置，则返回 DateTime.MinValue。

### 另见

* class [Task](../../task/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


