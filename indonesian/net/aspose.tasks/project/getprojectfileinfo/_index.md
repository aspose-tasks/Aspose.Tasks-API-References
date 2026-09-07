---
title: "Project.GetProjectFileInfo"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Project. Membaca info file proyek dari file"
type: docs
weight: 1280
url: /id/net/aspose.tasks/project/getprojectfileinfo/
---
## GetProjectFileInfo(string) {#getprojectfileinfo_1}

Membaca info file proyek dari file.

```csharp
public static ProjectFileInfo GetProjectFileInfo(string filename)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama file | String | Nama file proyek. |

### Nilai Kembali

Info file proyek [`ProjectFileInfo`](../../projectfileinfo/).

## Contoh

Menampilkan cara membaca info file proyek yang dibaca dari file XML.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Lihat Juga

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetProjectFileInfo(Stream) {#getprojectfileinfo}

Mengambil info file proyek dari aliran.

```csharp
public static ProjectFileInfo GetProjectFileInfo(Stream stream)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | Aliran data. |

### Nilai Kembali

Info file proyek [`ProjectFileInfo`](../../projectfileinfo/).

## Contoh

Menampilkan cara membaca informasi file proyek dari file XML yang dibaca dari aliran.

```csharp
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var info = Project.GetProjectFileInfo(stream);
    Console.WriteLine("CanRead: " + info.CanRead);
    Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
    Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
}
```

### Lihat Juga

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


