---
title: "Tsk.Calendar"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。任务日历"
type: docs
weight: 160
url: /zh/net/aspose.tasks/tsk/calendar/
---
## Tsk.Calendar field

任务日历。

```csharp
public static readonly Key<Calendar, TaskKey> Calendar;
```

## 示例

展示如何读取/写入任务日历。

```csharp
var project = new Project(DataDir + "ReadTaskCalendar.mpp");
var task = project.RootTask.Children.Add("Task1");

// 创建日历并分配给任务
var newCalendar = project.Calendars.Add("TaskCal1");
task.Set(Tsk.Calendar, newCalendar);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// 解析所有递归子项
foreach (var tsk in collector.Tasks)
{
    var calendar = tsk.Get(Tsk.Calendar);
    Console.WriteLine("Task calendar name: {0}", calendar == null ? "None" : calendar.Name);
}
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


