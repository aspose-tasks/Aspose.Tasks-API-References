---
title: "Resource.GetTimephasedData"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Resource. Mengembalikan sebuah instance dari kelas TimephasedDataCollection untuk objek ini dengan nilai TimephasedData dalam rentang tanggal mulai dan akhir yang diberikan untuk TimephasedDataType yang ditentukan"
type: docs
weight: 850
url: /id/net/aspose.tasks/resource/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Mengembalikan sebuah instance dari kelas [`TimephasedDataCollection`](../../timephaseddatacollection/) untuk objek ini dengan nilai [`TimephasedData`](../timephaseddata/) dalam rentang tanggal mulai dan akhir yang diberikan untuk [`TimephasedDataType`](../../timephaseddatatype/) yang ditentukan.

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

Daftar [`TimephasedData`](../timephaseddata/).

## Contoh

Menampilkan cara membaca data berjangka waktu dari sumber daya kerja/biaya.

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// Dapatkan Resource berdasarkan ID-nya
var resource = project.Resources.GetByUid(1);

// Cetak data berjangka waktu dari ResourceWork
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// Cetak data berjangka waktu dari ResourceCost
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### Lihat Juga

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Mengembalikan [`TimephasedDataCollection`](../../timephaseddatacollection/) untuk objek ini dengan nilai [`TimephasedData`](../timephaseddata/) dalam rentang tanggal mulai dan akhir yang diberikan.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| mulai | DateTime | Tanggal mulai untuk data berjangka waktu. |
| akhir | DateTime | Tanggal akhir untuk data berjangka waktu. |

### Nilai Kembali

Daftar [`TimephasedData`](../../timephaseddata/).

## Contoh

Menampilkan cara membaca data berjangka waktu dari sumber daya kerja/biaya.

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// Dapatkan Resource berdasarkan ID-nya
var resource = project.Resources.GetByUid(1);

// Cetak data berjangka waktu dari ResourceWork
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// Cetak data berjangka waktu dari ResourceCost
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### Lihat Juga

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


