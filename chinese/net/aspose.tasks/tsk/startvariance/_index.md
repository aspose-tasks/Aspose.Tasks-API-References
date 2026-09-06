---
title: "Tsk.StartVariance"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。表示任务或分配的基准开始日期与当前计划开始日期之间差异的时间"
type: docs
weight: 1040
url: /zh/net/aspose.tasks/tsk/startvariance/
---
## Tsk.StartVariance field

表示任务或分配的基准开始日期与当前计划开始日期之间差异的时间。

```csharp
public static readonly Key<Duration, TaskKey> StartVariance;
```

## 示例

展示如何读取/写入 Tsk.StartVariance 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Start Variance: " + task.Get(Tsk.StartVariance));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


