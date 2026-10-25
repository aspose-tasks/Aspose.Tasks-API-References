---
title: "Prj.ScheduleFromStart"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。确定是否从开始日期向前计算项目进度表"
type: docs
weight: 630
url: /zh/net/aspose.tasks/prj/schedulefromstart/
---
## Prj.ScheduleFromStart field

确定是否从开始日期向前计算项目进度表。

```csharp
public static readonly Key<NullableBool, PrjKey> ScheduleFromStart;
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
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


