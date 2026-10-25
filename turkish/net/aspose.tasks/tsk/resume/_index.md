---
title: "Tsk.Resume"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin kalan kısmının ilerleme girildikten sonra yeniden başlatılması için planlanan tarih"
type: docs
weight: 1000
url: /tr/net/aspose.tasks/tsk/resume/
---
## Tsk.Resume field

Görevin kalan kısmının ilerleme kaydedildikten sonra yeniden başlaması planlanan tarih.

```csharp
public static readonly Key<DateTime, TaskKey> Resume;
```

## Örnekler

Görevin Stop/Resume tarihlerini okuma nasıl gösterir.

```csharp
var project = new Project(DataDir + "StopResumeDates.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Tüm görevler için Stop ve Resume tarihlerini kontrol edin
foreach (var task in collector.Tasks)
{
    if (task.Get(Tsk.Stop).ToShortDateString() == "1/1/2000")
    {
        Console.WriteLine("Stop: NA");
    }
    else
    {
        Console.WriteLine("Stop: " + task.Get(Tsk.Stop).ToShortDateString());
    }

    if (task.Get(Tsk.Resume).ToShortDateString() == "1/1/2000")
    {
        Console.WriteLine("Resume: NA");
    }
    else
    {
        Console.WriteLine("Resume: " + task.Get(Tsk.Resume).ToShortDateString());
    }
}
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


