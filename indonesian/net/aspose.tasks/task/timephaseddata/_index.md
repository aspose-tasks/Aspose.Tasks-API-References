---
title: "Task.TimephasedData"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Task. Mendapatkan atau mengatur objek TimephasedDataCollection dari task ini. Blok data berwaktu yang terkait dengan sebuah task"
type: docs
weight: 1220
url: /id/net/aspose.tasks/task/timephaseddata/
---
## Task.TimephasedData property

Mendapatkan atau mengatur objek TimephasedDataCollection dari tugas ini. Blok data berfase waktu yang terkait dengan sebuah tugas.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Catatan

Pembacaan hanya didukung untuk format XML.

## Contoh

Menampilkan cara mengiterasi data berwaktu task.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");
var task = project.RootTask.Children.GetById(1);

foreach (var td in task.TimephasedData)
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


