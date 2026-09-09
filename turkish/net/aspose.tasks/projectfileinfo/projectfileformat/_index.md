---
title: "ProjectFileInfo.ProjectFileFormat"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectFileInfo özelliği. Proje dosyası biçimini alır"
type: docs
weight: 40
url: /tr/net/aspose.tasks/projectfileinfo/projectfileformat/
---
## ProjectFileInfo.ProjectFileFormat property

Proje dosyası formatını alır.

```csharp
public FileFormat ProjectFileFormat { get; }
```

## Örnekler

Proje dosyası bilgilerini nasıl okuyacağınızı gösterir.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Ayrıca Bakınız

* enum [FileFormat](../../fileformat/)
* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


