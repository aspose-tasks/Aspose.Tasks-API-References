---
title: "Tsk.PercentComplete"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。任务的当前状态，以已完成的任务持续时间百分比表示"
type: docs
weight: 880
url: /zh/net/aspose.tasks/tsk/percentcomplete/
---
## Tsk.PercentComplete field

任务的当前状态，以已完成的任务工期百分比表示。

```csharp
public static readonly Key<int, TaskKey> PercentComplete;
```

## 示例

展示如何通过更新任务完成百分比来更改任务进度。

```csharp
var project = new Project();
Console.WriteLine("Project Calculation mode is Automatic: {0}", project.CalculationMode.Equals(CalculationMode.Automatic));

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(2));
task.Set(Tsk.PercentComplete, 50);

// 访问任务并显示完成百分比
foreach (var tsk in project.RootTask.Children)
{
    Console.WriteLine(tsk.Get(Tsk.PercentComplete));
    Console.WriteLine(tsk.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(tsk.Get(Tsk.PhysicalPercentComplete));
}
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


