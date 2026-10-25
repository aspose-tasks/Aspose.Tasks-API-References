---
title: "ProjectFileInfo.CanRead"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectFileInfo özelliği. Proje dosyasını Aspose.Tasks işleyip işleyemeyeceğini gösteren bir değer alır."
type: docs
weight: 10
url: /tr/net/aspose.tasks/projectfileinfo/canread/
---
## ProjectFileInfo.CanRead property

Aspose.Tasks'in proje dosyasını işleyip işleyemeyeceğini gösteren bir değeri alır.

```csharp
public bool CanRead { get; }
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

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


