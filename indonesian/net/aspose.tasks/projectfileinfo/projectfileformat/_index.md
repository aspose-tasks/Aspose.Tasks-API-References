---
title: "ProjectFileInfo.ProjectFileFormat"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "ProjectFileInfo properti. Mendapatkan format file proyek"
type: docs
weight: 40
url: /id/net/aspose.tasks/projectfileinfo/projectfileformat/
---
## ProjectFileInfo.ProjectFileFormat property

Mendapatkan format file proyek.

```csharp
public FileFormat ProjectFileFormat { get; }
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

* enum [FileFormat](../../fileformat/)
* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


