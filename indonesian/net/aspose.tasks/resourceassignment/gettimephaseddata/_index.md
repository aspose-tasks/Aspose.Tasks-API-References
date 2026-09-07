---
title: "ResourceAssignment.GetTimephasedData"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ResourceAssignment. Mengembalikan instance kelas TimephasedDataCollection yang berisi instance kelas TimephasedData dalam rentang tanggal mulai dan akhir yang diberikan untuk TimephasedDataType yang ditentukan"
type: docs
weight: 720
url: /id/net/aspose.tasks/resourceassignment/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Mengembalikan instance kelas [`TimephasedDataCollection`](../../timephaseddatacollection/) yang berisi instance kelas [`TimephasedData`](../timephaseddata/) dalam rentang tanggal mulai dan akhir yang diberikan untuk [`TimephasedDataType`](../../timephaseddatatype/) yang ditentukan.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end, 
    TimephasedDataType timephasedType)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| mulai | DateTime | Tanggal mulai untuk data berjangka waktu. |
| akhir | DateTime | Tanggal akhir untuk data berjangka waktu. |
| timephasedType | TimephasedDataType | Tipe data berjangka waktu ([`TimephasedDataType`](../../timephaseddatatype/)). |

### Nilai Kembali

mengembalikan daftar yang berisi instance kelas [`TimephasedData`](../../timephaseddata/).

## Contoh

Menampilkan cara menghasilkan data timephased dari penugasan sumber daya dalam rentang tanggal.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// Atur properti proyek
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

// Atur kontur Backloaded, ini meningkatkan durasi tugas dari 6 menjadi 10 hari
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// dapatkan data timephased
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### Lihat Juga

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Mengembalikan objek [`TimephasedDataCollection`](../../timephaseddatacollection/) dengan instance kelas [`TimephasedData`](../timephaseddata/) dalam rentang tanggal mulai dan akhir yang diberikan untuk AssignmentWork.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| mulai | DateTime | Tanggal mulai untuk data berjangka waktu. |
| akhir | DateTime | Tanggal akhir untuk data berjangka waktu. |

### Nilai Kembali

mengembalikan daftar yang berisi instance kelas [`TimephasedData`](../../timephaseddata/).

## Contoh

Menampilkan cara menghasilkan data timephased dari penugasan sumber daya dalam rentang tanggal.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// Atur properti proyek
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

// Atur kontur Backloaded, ini meningkatkan durasi tugas dari 6 menjadi 10 hari
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// dapatkan data timephased
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### Lihat Juga

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


