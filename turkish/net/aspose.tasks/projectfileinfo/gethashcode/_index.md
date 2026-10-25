---
title: "ProjectFileInfo.GetHashCode"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectFileInfo yöntemi. ProjectFileInfo sınıfının örneği için bir karma kod değeri döndürür."
type: docs
weight: 60
url: /tr/net/aspose.tasks/projectfileinfo/gethashcode/
---
## ProjectFileInfo.GetHashCode method

[`ProjectFileInfo`](../) sınıfının örneği için bir karma kod değeri döndürür.

```csharp
public override int GetHashCode()
```

### Dönüş Değeri

bu nesne için bir karma kod değeri döndürür.

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


