---
title: "Kelas PrimaveraDbReader"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.PrimaveraDbReader. Mewakili pembaca untuk membaca Info Proyek dari Primavera DB."
type: docs
weight: 1350
url: /id/net/aspose.tasks/primaveradbreader/
---
## PrimaveraDbReader class

Mewakili pembaca untuk membaca Info Proyek dari DB Primavera.

```csharp
public sealed class PrimaveraDbReader : PrimaveraBaseReader
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [PrimaveraDbReader](primaveradbreader/)(PrimaveraDbSettings) | Menginisialisasi instance baru dari kelas [`PrimaveraXerReader`](../primaveraxerreader/). |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Kembalikan daftar objek info singkat proyek. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Kembalikan daftar pengidentifikasi unik proyek. |
| override [LoadProject](../../aspose.tasks/primaveradbreader/loadproject/)(int) | Muat proyek dengan pengidentifikasi unik yang ditentukan. |

## Contoh

Menampilkan cara mendapatkan info singkat proyek dari basis data Primavera.

```csharp
var settings = new PrimaveraDbSettings(GetConnectionString(), 0);

var reader = new PrimaveraDbReader(settings);
var projectInfos = reader.GetProjectInfos();

foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - '{2}'", info.Uid, info.ShortName, info.Name);
}

var firstProject = reader.LoadProject(projectInfos[0].Uid);
Console.WriteLine(firstProject.Uid);
Console.WriteLine(firstProject.Name);
Console.WriteLine(firstProject.PrimaveraProperties.ShortName);
```

### Lihat Juga

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


