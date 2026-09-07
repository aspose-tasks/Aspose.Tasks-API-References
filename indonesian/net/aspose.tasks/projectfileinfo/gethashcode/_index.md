---
title: "ProjectFileInfo.GetHashCode"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "ProjectFileInfo metode. Mengembalikan nilai kode hash untuk instance dari kelas ProjectFileInfo"
type: docs
weight: 60
url: /id/net/aspose.tasks/projectfileinfo/gethashcode/
---
## ProjectFileInfo.GetHashCode method

Mengembalikan nilai kode hash untuk instance dari kelas [`ProjectFileInfo`](../).

```csharp
public override int GetHashCode()
```

### Nilai Kembali

mengembalikan nilai kode hash untuk objek ini.

## Contoh

Menampilkan cara membaca informasi file proyek.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Lihat Juga

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


