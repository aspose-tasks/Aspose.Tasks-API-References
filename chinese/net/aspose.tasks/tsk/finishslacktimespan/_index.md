---
title: "Tsk.FinishSlackTimeSpan"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。早完成日期和晚完成日期之间的持续时间"
type: docs
weight: 400
url: /zh/net/aspose.tasks/tsk/finishslacktimespan/
---
## Tsk.FinishSlackTimeSpan field

最早完成日期与最迟完成日期之间的持续时间。

```csharp
public static readonly Key<TimeSpan, TaskKey> FinishSlackTimeSpan;
```

## 示例

展示如何读取 Tsk.FinishSlackTimeSpan 属性。该属性是计算得出的，通常无需显式设置。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Finish Slack: " + task.Get(Tsk.FinishSlackTimeSpan));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


