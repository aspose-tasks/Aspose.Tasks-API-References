---
title: "Task.GetTimephasedData"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Task. Mengembalikan objek TimephasedDataCollection dengan nilai TimephasedData dalam rentang tanggal mulai dan selesai yang diberikan untuk tipe data timephased yang ditentukan"
type: docs
weight: 1360
url: /id/net/aspose.tasks/task/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Mengembalikan objek [`TimephasedDataCollection`](../../timephaseddatacollection/) dengan nilai [`TimephasedData`](../timephaseddata/) dalam rentang tanggal mulai dan selesai yang diberikan untuk tipe data time-phased yang ditentukan.

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

Sebuah objek [`TimephasedDataCollection`](../../timephaseddatacollection/) dengan nilai [`TimephasedData`](../timephaseddata/) dalam rentang tanggal mulai dan selesai yang diberikan untuk tipe data timephased yang ditentukan.

## Contoh

Menampilkan cara mendapatkan data timephased (dengan tipe tertentu) dari tugas.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");
var task = project.RootTask.Children.GetById(1);

List<TimephasedData> data = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate).AddDays(2), TimephasedDataType.TaskBaselineWork)
    .ToList();
foreach (var td in data)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### Lihat Juga

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Mengembalikan objek [`TimephasedDataCollection`](../../timephaseddatacollection/) dengan nilai [`TimephasedData`](../timephaseddata/) dalam rentang tanggal mulai dan selesai yang diberikan.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| mulai | DateTime | Tanggal mulai untuk data berjangka waktu. |
| akhir | DateTime | Tanggal akhir untuk data berjangka waktu. |

### Nilai Kembali

Daftar [`TimephasedData`](../../timephaseddata/) yang harus diisi.

## Contoh

Menampilkan cara mendapatkan data berwaktu (dengan tipe TaskWork) dari tugas.

```csharp
var task = project.RootTask.Children.GetById(1);

List<TimephasedData> data = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)).ToList();
foreach (var td in data)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### Lihat Juga

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


