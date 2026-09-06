---
title: "Tsk.DurationVariance"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。任务的基准持续时间与当前估计的总持续时间之间的差异"
type: docs
weight: 320
url: /zh/net/aspose.tasks/tsk/durationvariance/
---
## Tsk.DurationVariance field

任务的基准持续时间与总持续时间（当前估计）之间的差额。

```csharp
public static readonly Key<Duration, TaskKey> DurationVariance;
```

## 示例

展示如何读取/写入 Tsk.DurationVariance 属性。

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationVariance, project.GetWork(1));

Console.WriteLine("Duration Variance: " + task.Get(Tsk.DurationVariance));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


