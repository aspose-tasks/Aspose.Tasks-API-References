---
title: "Tsk.StartVariance"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görev veya atamanın temel başlangıç tarihleri ile şu anda planlanan başlangıç tarihi arasındaki farkı temsil eden zaman."
type: docs
weight: 1040
url: /tr/net/aspose.tasks/tsk/startvariance/
---
## Tsk.StartVariance field

Bir görevin veya atamanın temel başlangıç tarihinin ve şu anda planlanan başlangıç tarihinin arasındaki farkı temsil eden zaman.

```csharp
public static readonly Key<Duration, TaskKey> StartVariance;
```

## Örnekler

Tsk.StartVariance özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Start Variance: " + task.Get(Tsk.StartVariance));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


