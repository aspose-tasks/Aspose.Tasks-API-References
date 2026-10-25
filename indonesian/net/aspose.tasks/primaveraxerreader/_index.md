---
title: "Kelas PrimaveraXerReader"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.PrimaveraXerReader. Mewakili pembaca untuk membaca UID Proyek dari file Primavera XER"
type: docs
weight: 1390
url: /id/net/aspose.tasks/primaveraxerreader/
---
## PrimaveraXerReader class

Mewakili pembaca untuk membaca UID Proyek dari file Primavera XER.

```csharp
public sealed class PrimaveraXerReader : PrimaveraBaseReader
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [PrimaveraXerReader](primaveraxerreader/#constructor)(Stream) | Menginisialisasi instance baru dari kelas `PrimaveraXerReader`. |
| [PrimaveraXerReader](primaveraxerreader/#constructor_1)(string) | Menginisialisasi instance baru dari kelas `PrimaveraXerReader`. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Kembalikan daftar objek info singkat proyek. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Kembalikan daftar pengidentifikasi unik proyek. |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | Muat proyek dengan pengidentifikasi unik yang ditentukan. |

## Contoh

Menampilkan cara memeriksa info proyek singkat dari file Primavera XER.

```csharp
var reader = new PrimaveraXerReader(DataDir + "MultiprojectWithExternal.xer");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}

var project = reader.LoadProject(5494);

Console.WriteLine("Loaded project '{0}' with Uid {1}", project.Name, project.Uid);
```

### Lihat Juga

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


