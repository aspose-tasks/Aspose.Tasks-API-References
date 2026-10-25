---
title: "Tsk.WorkVariance"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin temel iş miktarı ile şu anda planlanan iş arasındaki fark"
type: docs
weight: 1160
url: /tr/net/aspose.tasks/tsk/workvariance/
---
## Tsk.WorkVariance field

Bir görevin temel iş miktarı ile şu anda planlanan iş miktarı arasındaki fark.

```csharp
public static readonly Key<Duration, TaskKey> WorkVariance;
```

## Örnekler

Tsk.WorkVariance özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.WorkVariance, project.GetDuration(1));

Console.WriteLine("Work Variance: " + task.Get(Tsk.WorkVariance));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


