---
title: Calendar.GetTaskFinishDateFromDuration
second_title: Aspose.Tasks for .NET API 参考
description: Calendar 方法. 从开始日期拆分部分和持续时间计算任务完成日期和时间
type: docs
weight: 190
url: /zh/net/aspose.tasks/calendar/gettaskfinishdatefromduration/
---
## Calendar.GetTaskFinishDateFromDuration method

从开始日期、拆分部分和持续时间计算任务完成日期和时间。

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| task | Task | 获取完成日期的任务。 |
| duration | TimeSpan | 要拆分的任务持续时间。 |

### 返回值

任务的完成日期。

### 评论

如果任务是摘要、null 或其开始日期未设置，则返回 DateTime.MinValue。

### 也可以看看

* class [Task](../../task/)
* class [Calendar](../)
* 命名空间 [Aspose.Tasks](../../calendar/)
* 部件 [Aspose.Tasks](../../../)


