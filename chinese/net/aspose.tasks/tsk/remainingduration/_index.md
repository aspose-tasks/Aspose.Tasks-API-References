---
title: "Tsk.RemainingDuration"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk field. 完成任务未完成部分所需的时间."
type: docs
weight: 960
url: /zh/net/aspose.tasks/tsk/remainingduration/
---
## Tsk.RemainingDuration field

完成任务未完成部分所需的时间。

```csharp
public static readonly Key<Duration, TaskKey> RemainingDuration;
```

## 示例

展示如何读取/写入 Tsk.RemainingDuration 属性.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Remaining Duration: " + task.Get(Tsk.RemainingDuration));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


