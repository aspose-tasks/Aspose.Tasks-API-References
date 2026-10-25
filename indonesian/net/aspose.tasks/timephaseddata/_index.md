---
title: "Kelas TimephasedData"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.TimephasedData. Mewakili data berfase waktu"
type: docs
weight: 2590
url: /id/net/aspose.tasks/timephaseddata/
---
## TimephasedData class

Mewakili data berfase waktu.

```csharp
public class TimephasedData
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [TimephasedData](timephaseddata/)() | Menginisialisasi instance baru dari kelas `TimephasedData`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Finish](../../aspose.tasks/timephaseddata/finish/) { get; set; } | Mendapatkan atau mengatur tanggal selesai periode data berfase waktu. |
| [Start](../../aspose.tasks/timephaseddata/start/) { get; set; } | Mendapatkan atau mengatur tanggal mulai periode data berfase waktu. |
| [TimephasedDataType](../../aspose.tasks/timephaseddata/timephaseddatatype/) { get; set; } | Mendapatkan atau mengatur tipe data berfase waktu. |
| [Uid](../../aspose.tasks/timephaseddata/uid/) { get; set; } | Mendapatkan atau mengatur pengidentifikasi unik data berfase waktu |
| [Unit](../../aspose.tasks/timephaseddata/unit/) { get; set; } | Mendapatkan atau mengatur satuan waktu periode data berfase waktu. |
| [Value](../../aspose.tasks/timephaseddata/value/) { get; set; } | Mendapatkan atau mengatur nilai per satuan waktu untuk periode data berfase waktu. |
| [ValueToCost](../../aspose.tasks/timephaseddata/valuetocost/) { get; set; } | Mendapatkan instance Double yang mewakili nilai string objek ini. |
| [ValueToDuration](../../aspose.tasks/timephaseddata/valuetoduration/) { get; } | Mendapatkan instance TimeSpan yang mewakili nilai string objek ini. |
| [ValueToUnits](../../aspose.tasks/timephaseddata/valuetounits/) { get; } | Mendapatkan instance Double yang mewakili nilai string objek ini untuk data berfase waktu berbasis satuan. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| static [CreateCostTimephased](../../aspose.tasks/timephaseddata/createcosttimephased/#createcosttimephased)(int, DateTime, DateTime, double, TimephasedDataType) | Membuat dan menginisialisasi instance baru dari kelas `TimephasedData` untuk data berfase waktu berbasis biaya. |
| static [CreateCostTimephased](../../aspose.tasks/timephaseddata/createcosttimephased/#createcosttimephased_1)(int, DateTime, DateTime, double, TimeUnitType, TimephasedDataType) | Membuat dan menginisialisasi instance baru dari kelas `TimephasedData` untuk data berfase waktu berbasis biaya. |
| static [CreateUnitTimephased](../../aspose.tasks/timephaseddata/createunittimephased/)(int, DateTime, DateTime, double, TimephasedDataType) | Membuat dan menginisialisasi instance baru dari kelas `TimephasedData` untuk data berfase waktu berbasis satuan dari penugasan sumber daya material. |
| static [CreateWorkTimephased](../../aspose.tasks/timephaseddata/createworktimephased/)(int, DateTime, DateTime, TimeSpan, TimeUnitType, TimephasedDataType) | Membuat dan menginisialisasi sebuah instance baru dari kelas `TimephasedData` untuk data berjangka waktu berbasis kerja. |

## Contoh

Menampilkan cara bekerja dengan data timephased khusus.

```csharp
var project = new Project(DataDir + "Project1.mpp") { CalculationMode = CalculationMode.None };

var workResource = project.Resources.Add("Work Resource");
workResource.Set(Rsc.Type, ResourceType.Work);
var costResource = project.Resources.Add("Cost Resource");
costResource.Set(Rsc.Type, ResourceType.Cost);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2018, 1, 1, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

var workAssignment = project.ResourceAssignments.Add(task, workResource);
workAssignment.Set(Asn.WorkContour, WorkContourType.Contoured);
var costAssignment = project.ResourceAssignments.Add(task, costResource);
costAssignment.Set(Asn.WorkContour, WorkContourType.Contoured);

// mari tambahkan tds timephased khusus
workAssignment.TimephasedData.Clear();

// tambahkan hari kerja
var td1 = TimephasedData.CreateWorkTimephased(
    workAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    TimeSpan.FromHours(40),
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentRemainingWork);

// tambahkan akhir pekan
var td2 = TimephasedData.CreateWorkTimephased(
    workAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 6, 8, 0, 0),
    new DateTime(2018, 1, 8, 8, 0, 0),
    TimeSpan.Zero,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentRemainingWork);

workAssignment.TimephasedData.Add(td1);
workAssignment.TimephasedData.Add(td2);

costAssignment.TimephasedData.Clear();

// tambahkan hari kerja
var td11 = TimephasedData.CreateCostTimephased(
    costAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    1,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentCost);

// tambahkan akhir pekan
var td22 = TimephasedData.CreateCostTimephased(
    costAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 6, 8, 0, 0),
    new DateTime(2018, 1, 8, 8, 0, 0),
    0,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentCost);

costAssignment.TimephasedData.Add(td11);
costAssignment.TimephasedData.Add(td22);

Console.WriteLine("Print assignment timephased data:");
foreach (var assignment in project.ResourceAssignments)
{
    Console.WriteLine("Assignment UID: " + assignment.Get(Asn.Uid));
    foreach (var tds in assignment.TimephasedData)
    {
        Console.WriteLine("  Uid: " + tds.Uid);
        Console.WriteLine("  Start: " + tds.Start);
        Console.WriteLine("  Finish: " + tds.Finish);
        Console.WriteLine("  Type: " + tds.TimephasedDataType);
        Console.WriteLine("  Unit: " + tds.Unit);
        Console.WriteLine("  Value: " + tds.Value);
        Console.WriteLine("  ValueToCost: " + tds.ValueToCost);
        Console.WriteLine("  ValueToDuration: " + tds.ValueToDuration);
        Console.WriteLine("  ValueToUnits: " + tds.ValueToUnits);
        Console.WriteLine();
    }
}

project.Recalculate();
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


