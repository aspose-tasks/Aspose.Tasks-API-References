---
title: "Tsk.Stop"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。表示任务实际部分结束的日期"
type: docs
weight: 1060
url: /zh/net/aspose.tasks/tsk/stop/
---
## Tsk.Stop field

表示任务实际部分结束的日期。

```csharp
public static readonly Key<DateTime, TaskKey> Stop;
```

## 示例

展示如何读取任务的 Stop/Resume 日期。

```csharp
var project = new Project(DataDir + "StopResumeDates.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// 检查所有任务的 Stop 和 Resume 日期
foreach (var task in collector.Tasks)
{
    if (task.Get(Tsk.Stop).ToShortDateString() == "1/1/2000")
    {
        Console.WriteLine("Stop: NA");
    }
    else
    {
        Console.WriteLine("Stop: " + task.Get(Tsk.Stop).ToShortDateString());
    }

    if (task.Get(Tsk.Resume).ToShortDateString() == "1/1/2000")
    {
        Console.WriteLine("Resume: NA");
    }
    else
    {
        Console.WriteLine("Resume: " + task.Get(Tsk.Resume).ToShortDateString());
    }
}
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


