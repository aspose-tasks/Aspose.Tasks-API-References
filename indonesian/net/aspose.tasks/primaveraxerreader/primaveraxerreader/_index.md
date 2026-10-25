---
title: "PrimaveraXerReader.PrimaveraXerReader"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor PrimaveraXerReader. Menginisialisasi instance baru dari kelas PrimaveraXerReader"
type: docs
weight: 10
url: /id/net/aspose.tasks/primaveraxerreader/primaveraxerreader/
---
## PrimaveraXerReader(string) {#constructor_1}

Menginisialisasi instance baru dari kelas [`PrimaveraXerReader`](../).

```csharp
public PrimaveraXerReader(string xerFilePath)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| xerFilePath | String | Jalur ke file .xer tempat proyek Primavera atau proyek-proyek berada. |

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

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXerReader(Stream) {#constructor}

Menginisialisasi instance baru dari kelas [`PrimaveraXerReader`](../).

```csharp
public PrimaveraXerReader(Stream stream)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | Stream dengan konten XER Primavera. |

### Lihat Juga

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)


