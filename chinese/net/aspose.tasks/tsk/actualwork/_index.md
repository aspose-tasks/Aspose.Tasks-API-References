---
title: "Tsk.ActualWork"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。已由分配给任务的资源完成的工作量"
type: docs
weight: 90
url: /zh/net/aspose.tasks/tsk/actualwork/
---
## Tsk.ActualWork field

已由分配到任务的资源完成的工作量。

```csharp
public static readonly Key<Duration, TaskKey> ActualWork;
```

## 示例

展示如何读取/写入 Tsk.ActualWork 属性。

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + task.Get(Tsk.ActualWork));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


