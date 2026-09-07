---
title: "Kelas TimephasedDataCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.TimephasedDataCollection. Mewakili koleksi objek TimephasedData"
type: docs
weight: 2600
url: /id/net/aspose.tasks/timephaseddatacollection/
---
## TimephasedDataCollection class

Mewakili koleksi objek [`TimephasedData`](../timephaseddata/).

```csharp
public abstract class TimephasedDataCollection : IList<TimephasedData>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../aspose.tasks/timephaseddatacollection/count/) { get; } | Mendapatkan jumlah objek yang terkandung dalam objek `TimephasedDataCollection` ini. |
| [IsReadOnly](../../aspose.tasks/timephaseddatacollection/isreadonly/) { get; } | Mendapatkan nilai yang menunjukkan apakah ICollection bersifat read-only. |
| [Item](../../aspose.tasks/timephaseddatacollection/item/) { get; set; } | Mengembalikan elemen pada indeks yang ditentukan. Akses set tidak didukung. properti untuk mengatur data timephased. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Add](../../aspose.tasks/timephaseddatacollection/add/)(TimephasedData) | Menambahkan instance [`TimephasedData`](../timephaseddata/) ke objek koleksi ini. |
| [AddRange](../../aspose.tasks/timephaseddatacollection/addrange/)(IEnumerable&lt;TimephasedData&gt;) | Menambahkan koleksi instance [`TimephasedData`](../timephaseddata/) ke objek koleksi ini. |
| [Clear](../../aspose.tasks/timephaseddatacollection/clear/)() | Menghapus semua item dari `TimephasedDataCollection`. |
| [Contains](../../aspose.tasks/timephaseddatacollection/contains/)(TimephasedData) | Menentukan apakah `TimephasedDataCollection` berisi nilai tertentu. |
| [CopyTo](../../aspose.tasks/timephaseddatacollection/copyto/)(TimephasedData[], int) | Menyalin elemen `TimephasedDataCollection` ke sebuah Array, mulai pada indeks Array tertentu. |
| [GetEnumerator](../../aspose.tasks/timephaseddatacollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [Remove](../../aspose.tasks/timephaseddatacollection/remove/)(TimephasedData) | Menghapus instance [`TimephasedData`](../timephaseddata/) dari objek koleksi ini. |
| [SelectBetweenStartAndFinish](../../aspose.tasks/timephaseddatacollection/selectbetweenstartandfinish/)(TimephasedDataType, DateTime, DateTime) | Memilih semua fase waktu antara *startTime* dan *finishTime*. Memiliki kompleksitas O(log n) dalam kasus rata-rata. |
| [ToList](../../aspose.tasks/timephaseddatacollection/tolist/)() | Mengonversi objek `TimephasedDataCollection` menjadi daftar objek [`TimephasedData`](../timephaseddata/). |

## Contoh

Menampilkan cara bekerja dengan koleksi data timephased.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var resource2 = project.Resources.Add("Resource 2");
resource2.Set(Rsc.Type, ResourceType.Work);

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2019, 11, 11, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.Work, project.GetDuration(3d, TimeUnitType.Hour));
task.Set(Tsk.Finish, new DateTime(2019, 11, 13, 17, 0, 0));

var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2019, 11, 11, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task2.Set(Tsk.Work, project.GetDuration(3d, TimeUnitType.Hour));
task2.Set(Tsk.Finish, new DateTime(2019, 11, 13, 17, 0, 0));

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Start, new DateTime(2019, 11, 11, 8, 0, 0));
assignment.Set(Asn.Work, project.GetDuration(3, TimeUnitType.Hour));
assignment.Set(Asn.Finish, new DateTime(2019, 11, 13, 17, 0, 0));

var assignment2 = project.ResourceAssignments.Add(task2, resource2);
assignment2.Set(Asn.Start, new DateTime(2019, 11, 11, 8, 0, 0));
assignment2.Set(Asn.Work, project.GetDuration(3, TimeUnitType.Hour));
assignment2.Set(Asn.Finish, new DateTime(2019, 11, 13, 17, 0, 0));

// atur kontur kerja berkontur
assignment.Set(Asn.WorkContour, WorkContourType.Contoured);

Console.WriteLine("Is timephased data collection read-only?: " + assignment.TimephasedData.IsReadOnly);

// hapus tds yang dihasilkan
assignment.TimephasedData.Clear();

var td = new TimephasedData
             {
                 Start = new DateTime(2019, 11, 11, 8, 0, 0),
                 Finish = new DateTime(2019, 11, 11, 9, 0, 0),
                 Uid = assignment.Get(Asn.Uid),
                 Unit = TimeUnitType.Hour,
                 Value = "PT1H0M0S",
                 TimephasedDataType = TimephasedDataType.AssignmentRemainingWork
             };
assignment.TimephasedData.Add(td);

var list = new List<TimephasedData>();
var td2 = new TimephasedData
              {
                  Start = new DateTime(2019, 11, 12, 8, 0, 0),
                  Finish = new DateTime(2019, 11, 12, 9, 0, 0),
                  Uid = assignment.Get(Asn.Uid),
                  Unit = TimeUnitType.Hour,
                  Value = "PT1H0M0S",
                  TimephasedDataType = TimephasedDataType.AssignmentRemainingWork
              };
var td3 = new TimephasedData
              {
                  Start = new DateTime(2019, 11, 13, 8, 0, 0),
                  Finish = new DateTime(2019, 11, 13, 9, 0, 0),
                  Uid = assignment.Get(Asn.Uid),
                  Unit = TimeUnitType.Hour,
                  Value = "PT1H0M0S",
                  TimephasedDataType = TimephasedDataType.AssignmentRemainingWork
              };

list.Add(td2);
list.Add(td3);
assignment.TimephasedData.AddRange(list);

// seseorang dapat memfilter koleksi berdasarkan tipe dan rentang tanggal
Console.WriteLine("Print filtered tds:");
IList<TimephasedData> filteredTds = assignment.TimephasedData.SelectBetweenStartAndFinish(
    TimephasedDataType.AssignmentRemainingWork,
    new DateTime(2019, 11, 11, 0, 0, 0),
    new DateTime(2019, 11, 13));
foreach (var data in filteredTds)
{
    Console.WriteLine("Start: " + data.Start);
    Console.WriteLine("Finish: " + data.Finish);
    Console.WriteLine("Timephased Data Type: " + data.TimephasedDataType);
    Console.WriteLine();
}

Console.WriteLine("--------------------------");
Console.WriteLine();

// ...
// tambahkan td yang salah lalu hapus itu
var td4 = new TimephasedData
              {
                  Start = new DateTime(2019, 11, 13, 8, 0, 0),
                  Finish = new DateTime(2019, 11, 13, 9, 0, 0),
                  Uid = assignment.Get(Asn.Uid),
                  Unit = TimeUnitType.Hour,
                  Value = "PT0H0M1S", // wrong value
                  TimephasedDataType = TimephasedDataType.AssignmentRemainingWork
              };
assignment.TimephasedData.Add(td4);

// ...

// hapus item td yang salah
if (assignment.TimephasedData.Contains(td4))
{
    assignment.TimephasedData.Remove(td4);
}

// ...
assignment.TimephasedData.AddRange(list);

// iterasi melalui item timephased
Console.WriteLine("Print all timephased items:");
Console.WriteLine("Timephased data count: " + assignment.TimephasedData.Count);
foreach (var item in assignment.TimephasedData)
{
    Console.WriteLine("Start: " + item.Start);
    Console.WriteLine("Finish: " + item.Finish);
    Console.WriteLine("Timephased Data Type: " + item.TimephasedDataType);
    Console.WriteLine();
}

// salin tds ke penugasan lain
var timephasedDatas = new TimephasedData[assignment.TimephasedData.Count];
assignment.TimephasedData.CopyTo(timephasedDatas, 0);

assignment2.TimephasedData.Clear();
foreach (var data in timephasedDatas)
{
    assignment2.TimephasedData.Add(data);
}

// koleksi dapat dikonversi menjadi daftar biasa
List<TimephasedData> tds = assignment.TimephasedData.ToList();

// mari hapus tds satu per satu
foreach (var timephasedData in tds)
{
    assignment.TimephasedData.Remove(timephasedData);
}
```

### Lihat Juga

* class [TimephasedData](../timephaseddata/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


