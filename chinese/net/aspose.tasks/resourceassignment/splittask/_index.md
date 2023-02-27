---
title: ResourceAssignment.SplitTask
second_title: Aspose.Tasks for .NET API 参考
description: ResourceAssignment 方法. 将任务分成两部分
type: docs
weight: 750
url: /zh/net/aspose.tasks/resourceassignment/splittask/
---
## ResourceAssignment.SplitTask method

将任务分成两部分。

```csharp
public void SplitTask(DateTime start, DateTime finish, Calendar calendar)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| start | DateTime | 开始时以工作中断为依据进行拆分。 |
| finish | DateTime | 以工作中断结束为依据进行拆分。 |
| calendar | Calendar | 拆分所依据的日历。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentOutOfRangeException | 当开始日期小于分配开始日期时抛出。 |
| ArgumentOutOfRangeException | 当完成日期大于分配完成日期时抛出。 |

### 也可以看看

* class [Calendar](../../calendar/)
* class [ResourceAssignment](../)
* 命名空间 [Aspose.Tasks](../../resourceassignment/)
* 部件 [Aspose.Tasks](../../../)


