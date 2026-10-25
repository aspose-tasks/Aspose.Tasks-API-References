---
title: "ProjectFileInfo.ProjectApplicationInfo"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectFileInfo özelliği. Proje dosyası uygulama bilgilerini alır."
type: docs
weight: 30
url: /tr/net/aspose.tasks/projectfileinfo/projectapplicationinfo/
---
## ProjectFileInfo.ProjectApplicationInfo property

Proje dosyası uygulama bilgisini alır.

```csharp
public ApplicationInfo ProjectApplicationInfo { get; }
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

* enum [ApplicationInfo](../../applicationinfo/)
* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


