---
title: "ResourceAssignment.GetTimephasedData"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ResourceAssignment yöntemi. Belirtilen TimephasedDataType için verilen başlangıç ve bitiş tarihleri içinde TimephasedData sınıfının örneklerini içeren TimephasedDataCollection sınıfının örneğini döndürür."
type: docs
weight: 720
url: /tr/net/aspose.tasks/resourceassignment/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Belirtilen [`TimephasedDataType`](../../timephaseddatatype/) için verilen başlangıç ve bitiş tarihleri içinde [`TimephasedData`](../timephaseddata/) sınıfının örneklerini içeren [`TimephasedDataCollection`](../../timephaseddatacollection/) sınıfının örneğini döndürür.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end, 
    TimephasedDataType timephasedType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlangıç | DateTime | Zaman aşamalı veri için başlangıç tarihi. |
| bitiş | DateTime | Zaman aşamalı veri için bitiş tarihi. |
| timephasedType | TimephasedDataType | Zaman aşamalı veri türü ([`TimephasedDataType`](../../timephaseddatatype/)). |

### Dönüş Değeri

[`TimephasedData`](../../timephaseddata/) sınıfının örneklerini içeren bir liste döndürür.

## Örnekler

Bir tarih aralığında bir kaynak atamasının zaman aşamalı verilerini nasıl oluşturacağını gösterir.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// Proje özelliklerini ayarla
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

// Backloaded konturu ayarla, görev süresini 6 günden 10 güne artırır
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// zaman aşamalı veriyi al
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### Ayrıca Bakınız

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

AssignmentWork'un verilen başlangıç ve bitiş tarihleri içinde [`TimephasedData`](../timephaseddata/) sınıfının örneklerini içeren [`TimephasedDataCollection`](../../timephaseddatacollection/) nesnesini döndürür.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlangıç | DateTime | Zaman aşamalı veri için başlangıç tarihi. |
| bitiş | DateTime | Zaman aşamalı veri için bitiş tarihi. |

### Dönüş Değeri

[`TimephasedData`](../../timephaseddata/) sınıfının örneklerini içeren bir liste döndürür.

## Örnekler

Bir tarih aralığında bir kaynak atamasının zaman aşamalı verilerini nasıl oluşturacağını gösterir.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// Proje özelliklerini ayarla
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

// Backloaded konturu ayarla, görev süresini 6 günden 10 güne artırır
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// zaman aşamalı veriyi al
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### Ayrıca Bakınız

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


