---
title: "Tsk.EarlyFinish"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。任务可能完成的最早日期，基于前置任务和后续任务的早完成日期、其他约束以及任何平衡延迟"
type: docs
weight: 330
url: /zh/net/aspose.tasks/tsk/earlyfinish/
---
## Tsk.EarlyFinish field

基于前置和后续任务的最早完成日期、其他约束以及任何平衡延迟，任务可能完成的最早日期。

```csharp
public static readonly Key<DateTime, TaskKey> EarlyFinish;
```

## 示例

展示如何读取/写入 Tsk.EarlyFinish 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Finish: " + task.Get(Tsk.EarlyFinish));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


