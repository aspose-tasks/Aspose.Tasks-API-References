---
title: "PrimaveraXmlReader.PrimaveraXmlReader"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor PrimaveraXmlReader. Menginisialisasi instance baru dari kelas PrimaveraXmlReader"
type: docs
weight: 10
url: /id/net/aspose.tasks/primaveraxmlreader/primaveraxmlreader/
---
## PrimaveraXmlReader(string) {#constructor_1}

Menginisialisasi instance baru dari kelas [`PrimaveraXmlReader`](../).

```csharp
public PrimaveraXmlReader(string templatePath)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| templatePath | String | Jalur ke templat tempat proyek Primavera Xml atau proyek-proyek berada |

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

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXmlReader(Stream) {#constructor}

Menginisialisasi instance baru dari kelas [`PrimaveraXmlReader`](../).

```csharp
public PrimaveraXmlReader(Stream stream)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | Aliran yang berisi konten Primavera Xml. |

## Contoh

Menampilkan cara mengimpor proyek dari aliran Primavera XML.

```csharp
using (var stream = new FileStream(DataDir + "primavera.xml", FileMode.Open))
{
    var reader = new PrimaveraXmlReader(stream);
    List<int> projectUids = reader.GetProjectUids();
    foreach (var projectUid in projectUids)
    {
        Console.WriteLine("Project UID: " + projectUid);
    }
}
```

### Lihat Juga

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)


