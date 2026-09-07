---
title: "ResourceAssignment.MakeTPs"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "ResourceAssignment metode. Menghasilkan daftar data berfase waktu."
type: docs
weight: 740
url: /id/net/aspose.tasks/resourceassignment/maketps/
---
## ResourceAssignment.MakeTPs method

Menghasilkan daftar data berwaktu fase.

```csharp
public DateTime MakeTPs(DateTime start, TimeSpan time, Calendar calendar, 
    List<TimephasedData> list, bool isWorking, int type)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| mulai | DateTime | Tanggal mulai yang ditentukan. |
| waktu | TimeSpan | Waktu kerja yang ditentukan. |
| kalender | Calendar | Kalender kerja yang ditentukan. |
| daftar | List`1 | Daftar data berfase waktu. |
| isWorking | Boolean | Bendera yang ditentukan yang menunjukkan apakah data berfase waktu sedang bekerja atau tidak. |
| tipe | Int32 | Tipe data berfase waktu yang ditentukan. |

### Nilai Kembali

Tanggal maksimum dari daftar atau tanggal mulai jika daftar kosong.

## Contoh

Menampilkan cara menghasilkan TPs dengan parameter.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 3, 30, 8, 0, 0));
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Start, new DateTime(2020, 4, 1, 8, 0, 0));

var tps = new List<TimephasedData>();
var lastDate = assignment.MakeTPs(
    assignment.Get(Asn.Start),
    TimeSpan.FromHours(32),
    project.Calendars.GetByName("Standard"),
    tps,
    true,
    (int)TimephasedDataType.AssignmentRemainingWork);

foreach (var data in tps)
{
    Console.WriteLine("Start: " + data.Start);
    Console.WriteLine("Finish: " + data.Finish);
    Console.WriteLine("TimephasedDataType: " + data.TimephasedDataType);
    Console.WriteLine();
}
```

### Lihat Juga

* class [Calendar](../../calendar/)
* class [TimephasedData](../../timephaseddata/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


