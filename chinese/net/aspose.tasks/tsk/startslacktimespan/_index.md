---
title: "Tsk.StartSlackTimeSpan"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。早开始日期和晚开始日期之间的持续时间"
type: docs
weight: 1020
url: /zh/net/aspose.tasks/tsk/startslacktimespan/
---
## Tsk.StartSlackTimeSpan field

早开始和晚开始日期之间的持续时间。

```csharp
public static readonly Key<TimeSpan, TaskKey> StartSlackTimeSpan;
```

## 示例

展示如何读取 Tsk.StartSlackTimeSpan 属性。该属性是计算得出的，通常不需要显式设置。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Start Slack: " + task.Get(Tsk.StartSlackTimeSpan));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


