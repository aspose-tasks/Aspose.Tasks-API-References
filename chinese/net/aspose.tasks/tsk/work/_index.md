---
title: "Tsk.Work"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。任务上为所有指派资源计划的总时间"
type: docs
weight: 1150
url: /zh/net/aspose.tasks/tsk/work/
---
## Tsk.Work field

为所有分配资源在任务上计划的总时间。

```csharp
public static readonly Key<Duration, TaskKey> Work;
```

## 示例

展示如何读取/写入 Tsk.Work 属性。

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Work, project.GetWork(1));

Console.WriteLine("Work: " + task.Get(Tsk.Work));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


