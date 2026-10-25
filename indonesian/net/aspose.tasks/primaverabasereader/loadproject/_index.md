---
title: "PrimaveraBaseReader.LoadProject"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode PrimaveraBaseReader. Memuat proyek dengan identifier unik yang ditentukan"
type: docs
weight: 30
url: /id/net/aspose.tasks/primaverabasereader/loadproject/
---
## PrimaveraBaseReader.LoadProject method

Muat proyek dengan pengidentifikasi unik yang ditentukan.

```csharp
public virtual Project LoadProject(int projectUid)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| projectUid | Int32 | Pengidentifikasi unik dari proyek yang akan dimuat. |

### Nilai Kembali

Proyek dengan identifier unik yang ditentukan dari file multi proyek yang ditentukan. Null jika proyek tidak ada.

## Contoh

Menampilkan cara memuat proyek dari file XML Primavera ketika uid proyek diketahui.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "PrimaveraProject.xml");
var project = reader.LoadProject(3882);
Console.WriteLine(project.Name);
```

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

* class [Project](../../project/)
* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


