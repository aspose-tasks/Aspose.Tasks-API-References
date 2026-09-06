---
title: "Tsk.ActualOvertimeWork"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。已分配给任务的资源实际完成的加班工作量"
type: docs
weight: 60
url: /zh/net/aspose.tasks/tsk/actualovertimework/
---
## Tsk.ActualOvertimeWork field

已由分配到任务的资源完成的实际加班工作量。

```csharp
public static readonly Key<Duration, TaskKey> ActualOvertimeWork;
```

## 示例

展示如何读取/写入 Tsk.ActualOvertimeWork 属性。

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + task.Get(Tsk.ActualOvertimeWork));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


