---
title: "Tsk.RemainingOvertimeWork"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。剩余计划加班时间的数量。"
type: docs
weight: 980
url: /zh/net/aspose.tasks/tsk/remainingovertimework/
---
## Tsk.RemainingOvertimeWork field

剩余的计划加班时间量。

```csharp
public static readonly Key<Duration, TaskKey> RemainingOvertimeWork;
```

## 示例

展示如何读取/写入 Tsk.RemainingOvertimeWork 属性。

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + task.Get(Tsk.RemainingOvertimeWork));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


