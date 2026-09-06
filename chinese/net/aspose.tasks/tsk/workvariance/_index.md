---
title: "Tsk.WorkVariance"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk field. 任务基准工作量与当前计划工作量之间的差异."
type: docs
weight: 1160
url: /zh/net/aspose.tasks/tsk/workvariance/
---
## Tsk.WorkVariance field

任务基准工作量与当前计划工作量之间的差异。

```csharp
public static readonly Key<Duration, TaskKey> WorkVariance;
```

## 示例

展示如何读取/写入 Tsk.WorkVariance 属性.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.WorkVariance, project.GetDuration(1));

Console.WriteLine("Work Variance: " + task.Get(Tsk.WorkVariance));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


