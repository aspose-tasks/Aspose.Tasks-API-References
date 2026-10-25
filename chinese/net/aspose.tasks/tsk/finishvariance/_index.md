---
title: "Tsk.FinishVariance"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。表示任务或分配的基线完成日期与当前完成日期之间差异的时间"
type: docs
weight: 420
url: /zh/net/aspose.tasks/tsk/finishvariance/
---
## Tsk.FinishVariance field

表示任务或分配的基准完成日期与当前完成日期之间差异的时间。

```csharp
public static readonly Key<Duration, TaskKey> FinishVariance;
```

## 示例

展示如何读取/写入 Tsk.FinishVariance 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Finish Variance: " + task.Get(Tsk.FinishVariance));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


