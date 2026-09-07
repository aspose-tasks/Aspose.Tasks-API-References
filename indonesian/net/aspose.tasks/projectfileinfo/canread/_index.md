---
title: "ProjectFileInfo.CanRead"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "ProjectFileInfo properti. Mendapatkan nilai yang menunjukkan apakah Aspose.Tasks dapat memproses file proyek"
type: docs
weight: 10
url: /id/net/aspose.tasks/projectfileinfo/canread/
---
## ProjectFileInfo.CanRead property

Mendapatkan nilai yang menunjukkan apakah Aspose.Tasks dapat memproses file proyek.

```csharp
public bool CanRead { get; }
```

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


