---
title: "ProjectFileInfo.ProjectApplicationInfo"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ProjectFileInfo. Mendapatkan informasi aplikasi file proyek."
type: docs
weight: 30
url: /id/net/aspose.tasks/projectfileinfo/projectapplicationinfo/
---
## ProjectFileInfo.ProjectApplicationInfo property

Mendapatkan info aplikasi file proyek.

```csharp
public ApplicationInfo ProjectApplicationInfo { get; }
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

* enum [ApplicationInfo](../../applicationinfo/)
* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


