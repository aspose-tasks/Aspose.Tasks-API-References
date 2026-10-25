---
title: "ResourceAssignment.TimephasedData"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ResourceAssignment. Mendapatkan atau mengatur instance kelas TimephasedDataCollection yang berisi elemen-elemen kelas TimephasedData"
type: docs
weight: 600
url: /id/net/aspose.tasks/resourceassignment/timephaseddata/
---
## ResourceAssignment.TimephasedData property

Mendapatkan atau mengatur instance kelas [`TimephasedDataCollection`](../../timephaseddatacollection/) yang berisi elemen-elemen kelas `TimephasedData`.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Contoh

Menampilkan cara membaca data timephased dari penugasan sumber daya.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");
project.Set(Prj.StartDate, new DateTime(2013, 10, 30, 9, 0, 0));
project.Set(Prj.NewTasksAreManual, false);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(6));

var rsc = project.Resources.Add("Rsc");
rsc.Set(Rsc.StandardRate, 10);
rsc.Set(Rsc.OvertimeRate, 15);

// Buat penugasan sumber daya
var assn = project.ResourceAssignments.Add(task, rsc);
assn.Set(Asn.Stop, DateTime.MinValue);
assn.Set(Asn.Resume, DateTime.MinValue);
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

// dapatkan data timephased
foreach (var td in assn.TimephasedData)
{
    Console.WriteLine(td.Value);
}
```

### Lihat Juga

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


