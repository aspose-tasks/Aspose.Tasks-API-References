---
title: "Kelas PrimaveraXmlReader"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.PrimaveraXmlReader. Mewakili pembaca yang memungkinkan untuk mengambil UID Proyek dari file XML Primavera"
type: docs
weight: 1400
url: /id/net/aspose.tasks/primaveraxmlreader/
---
## PrimaveraXmlReader class

Mewakili pembaca yang memungkinkan mengambil UID Proyek dari file Primavera Xml.

```csharp
public class PrimaveraXmlReader : PrimaveraBaseReader
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor)(Stream) | Menginisialisasi instance baru dari kelas `PrimaveraXmlReader`. |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor_1)(string) | Menginisialisasi instance baru dari kelas `PrimaveraXmlReader`. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Kembalikan daftar objek info singkat proyek. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Kembalikan daftar pengidentifikasi unik proyek. |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | Muat proyek dengan pengidentifikasi unik yang ditentukan. |

## Contoh

Menampilkan cara memeriksa info proyek singkat dari file XML Primavera.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "MultiprojectWithExternal.xml");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}
```

### Lihat Juga

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


