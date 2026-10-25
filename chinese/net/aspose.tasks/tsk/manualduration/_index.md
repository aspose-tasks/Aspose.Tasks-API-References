---
title: "Tsk.ManualDuration"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。定义任务的手动计划持续时间"
type: docs
weight: 780
url: /zh/net/aspose.tasks/tsk/manualduration/
---
## Tsk.ManualDuration field

定义任务的手动计划工期。

```csharp
public static readonly Key<Duration, TaskKey> ManualDuration;
```

## 示例

展示如何读取/写入 Tsk.ManualDuration 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Manual Duration: " + task.Get(Tsk.ManualDuration));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


