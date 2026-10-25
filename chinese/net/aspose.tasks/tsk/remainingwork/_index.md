---
title: "Tsk.RemainingWork"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk field. 完成任务或任务集仍需的时间."
type: docs
weight: 990
url: /zh/net/aspose.tasks/tsk/remainingwork/
---
## Tsk.RemainingWork field

完成任务或任务集仍需的时间。

```csharp
public static readonly Key<Duration, TaskKey> RemainingWork;
```

## 示例

展示如何读取/写入 Tsk.RemainingWork 属性.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + task.Get(Tsk.RemainingWork));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


