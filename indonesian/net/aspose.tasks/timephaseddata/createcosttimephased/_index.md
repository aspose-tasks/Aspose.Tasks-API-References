---
title: "TimephasedData.CreateCostTimephased"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode TimephasedData. Membuat dan menginisialisasi instance baru dari kelas TimephasedData untuk data berwaktu fase berbasis biaya"
type: docs
weight: 20
url: /id/net/aspose.tasks/timephaseddata/createcosttimephased/
---
## CreateCostTimephased(int, DateTime, DateTime, double, TimeUnitType, TimephasedDataType) {#createcosttimephased_1}

Membuat dan menginisialisasi instance baru dari kelas [`TimephasedData`](../) untuk data berwaktu fase berbasis biaya.

```csharp
public static TimephasedData CreateCostTimephased(int uid, DateTime start, DateTime finish, 
    double value, TimeUnitType timeUnit, TimephasedDataType type)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| uid | Int32 | UID dari tugas. |
| mulai | DateTime | tanggal-waktu mulai. |
| selesai | DateTime | tanggal-waktu selesai. |
| value | Double | Nilai biaya. |
| timeUnit | TimeUnitType | Tipe satuan waktu. |
| tipe | TimephasedDataType | Tipe data berwaktu fase. |

### Nilai Kembali

Instance dari kelas [`TimephasedData`](../) untuk data berwaktu fase berbasis biaya.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | Jika nilai biaya negatif telah ditentukan. |

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

* enum [TimeUnitType](../../timeunittype/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* namespace [Aspose.Tasks](../../timephaseddata/)
* assembly [Aspose.Tasks](../../../)

---

## CreateCostTimephased(int, DateTime, DateTime, double, TimephasedDataType) {#createcosttimephased}

Membuat dan menginisialisasi instance baru dari kelas [`TimephasedData`](../) untuk data berwaktu fase berbasis biaya.

```csharp
public static TimephasedData CreateCostTimephased(int uid, DateTime start, DateTime finish, 
    double value, TimephasedDataType type)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| uid | Int32 | UID dari tugas. |
| mulai | DateTime | tanggal-waktu mulai. |
| selesai | DateTime | tanggal-waktu selesai. |
| value | Double | Nilai biaya. |
| tipe | TimephasedDataType | Tipe data berwaktu fase. |

### Nilai Kembali

Instance dari kelas [`TimephasedData`](../) untuk data berwaktu fase berbasis biaya.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | Jika nilai biaya negatif telah ditentukan. |

### Lihat Juga

* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* namespace [Aspose.Tasks](../../timephaseddata/)
* assembly [Aspose.Tasks](../../../)


