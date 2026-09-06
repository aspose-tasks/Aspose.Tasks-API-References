---
title: "Tsk.Duration"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。任务的总活跃工作时间跨度，既可以手动输入，也可以由 Microsoft Project 根据开始日期、结束日期、日历和其他调度因素计算得出"
type: docs
weight: 300
url: /zh/net/aspose.tasks/tsk/duration/
---
## Tsk.Duration field

任务的总活跃工作时间跨度，依据输入或 Microsoft Project 根据开始日期、完成日期、日历及其他调度因素计算得出。

```csharp
public static readonly Key<Duration, TaskKey> Duration;
```

## 示例

展示如何设置任务的持续时间。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddTaskDuration_out.xml", SaveFileFormat.Xml);
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


