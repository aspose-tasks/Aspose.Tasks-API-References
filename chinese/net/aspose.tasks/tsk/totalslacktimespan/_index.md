---
title: "Tsk.TotalSlackTimeSpan"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。任务完成日期可以延迟而不影响项目完成日期的时间"
type: docs
weight: 1090
url: /zh/net/aspose.tasks/tsk/totalslacktimespan/
---
## Tsk.TotalSlackTimeSpan field

任务完成日期可以延迟而不影响项目完成日期的时间。

```csharp
public static readonly Key<TimeSpan, TaskKey> TotalSlackTimeSpan;
```

## 示例

展示如何读取 Tsk.TotalSlackTimeSpan 属性。该属性是计算得出的，通常不需要显式设置。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Total Slack: " + task.Get(Tsk.TotalSlackTimeSpan));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


