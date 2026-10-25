---
title: "Prj.FinishDate"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。项目的完成日期"
type: docs
weight: 330
url: /zh/net/aspose.tasks/prj/finishdate/
---
## Prj.FinishDate field

项目的完成日期。

```csharp
public static readonly Key<DateTime, PrjKey> FinishDate;
```

## 示例

展示如何从完成日期而不是开始日期重新安排项目。

```csharp
var project = new Project();
project.Set(Prj.ScheduleFromStart, false);
project.Set(Prj.FinishDate, new DateTime(2020, 1, 1));

// 现在所有任务日期（Start、Finish、EarlyStart、EarlyFinish、LateStart、LateFinish）已计算。要获取关键路径，我们需要计算时差（可以在单独线程中调用，但必须在所有早/晚日期计算完成后）。
project.Recalculate();

foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id));
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


