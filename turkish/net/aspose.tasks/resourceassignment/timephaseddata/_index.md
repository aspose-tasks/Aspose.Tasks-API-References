---
title: "ResourceAssignment.TimephasedData"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ResourceAssignment özelliği. TimephasedData sınıfının öğelerini içeren TimephasedDataCollection sınıfının örneğini alır veya ayarlar"
type: docs
weight: 600
url: /tr/net/aspose.tasks/resourceassignment/timephaseddata/
---
## ResourceAssignment.TimephasedData property

TimephasedData sınıfının öğelerini içeren [`TimephasedDataCollection`](../../timephaseddatacollection/) sınıfının örneğini alır veya ayarlar.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Örnekler

Bir kaynak atamasının zaman aşamalı verilerini nasıl okuyacağını gösterir.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");
project.Set(Prj.StartDate, new DateTime(2013, 10, 30, 9, 0, 0));
project.Set(Prj.NewTasksAreManual, false);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(6));

var rsc = project.Resources.Add("Rsc");
rsc.Set(Rsc.StandardRate, 10);
rsc.Set(Rsc.OvertimeRate, 15);

// Kaynak ataması oluştur
var assn = project.ResourceAssignments.Add(task, rsc);
assn.Set(Asn.Stop, DateTime.MinValue);
assn.Set(Asn.Resume, DateTime.MinValue);
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

// zaman aşamalı veriyi al
foreach (var td in assn.TimephasedData)
{
    Console.WriteLine(td.Value);
}
```

### Ayrıca Bakınız

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


