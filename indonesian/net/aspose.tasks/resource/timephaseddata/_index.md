---
title: "Resource.TimephasedData"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Resource. Mendapatkan atau mengatur instance kelas TimephasedDataCollection untuk objek ini"
type: docs
weight: 740
url: /id/net/aspose.tasks/resource/timephaseddata/
---
## Resource.TimephasedData property

Mendapatkan atau mengatur sebuah instance dari kelas [`TimephasedDataCollection`](../../timephaseddatacollection/) untuk objek ini.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Catatan

Pembacaan hanya didukung untuk format XML.

## Contoh

Menampilkan cara membaca data timephased sumber daya.

```csharp
resource.Set(Rsc.Work, resource.ParentProject.GetWork(2));

project.SetBaseline(BaselineType.Baseline);

// iterasi atas data timephased dari sumber daya 
foreach (var td in resource.TimephasedData)
{
    Console.WriteLine(td.Start);
    Console.WriteLine(td.Finish);
}
```

### Lihat Juga

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


