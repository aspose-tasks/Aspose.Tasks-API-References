---
title: "Tsk.ManualFinish"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。定义任务的手动计划完成时间"
type: docs
weight: 790
url: /zh/net/aspose.tasks/tsk/manualfinish/
---
## Tsk.ManualFinish field

定义任务的手动计划完成时间。

```csharp
public static readonly Key<DateTime, TaskKey> ManualFinish;
```

## 示例

展示如何读取/写入 Tsk.ManualFinish 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Manual Finish: " + task.Get(Tsk.ManualFinish));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


