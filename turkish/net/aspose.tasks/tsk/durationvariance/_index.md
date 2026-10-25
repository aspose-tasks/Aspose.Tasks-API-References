---
title: "Tsk.DurationVariance"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin temel süresi ile mevcut toplam süre tahmini arasındaki fark."
type: docs
weight: 320
url: /tr/net/aspose.tasks/tsk/durationvariance/
---
## Tsk.DurationVariance field

Bir görevin temel süresi ile toplam süresi (güncel tahmin) arasındaki fark.

```csharp
public static readonly Key<Duration, TaskKey> DurationVariance;
```

## Örnekler

Tsk.DurationVariance özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationVariance, project.GetWork(1));

Console.WriteLine("Duration Variance: " + task.Get(Tsk.DurationVariance));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


