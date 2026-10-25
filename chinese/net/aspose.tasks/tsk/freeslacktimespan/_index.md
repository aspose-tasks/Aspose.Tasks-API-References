---
title: "Tsk.FreeSlackTimeSpan"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。任务可以延迟而不影响任何后续任务的时间"
type: docs
weight: 450
url: /zh/net/aspose.tasks/tsk/freeslacktimespan/
---
## Tsk.FreeSlackTimeSpan field

任务可以延迟而不影响任何后续任务的时间。

```csharp
public static readonly Key<TimeSpan, TaskKey> FreeSlackTimeSpan;
```

## 示例

展示如何读取 Tsk.FreeSlackTimeSpan 属性。该属性是计算得出的，通常不需要显式设置。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Free Slack: " + task.Get(Tsk.FreeSlackTimeSpan));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


