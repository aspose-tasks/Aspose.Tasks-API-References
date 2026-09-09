---
title: "Sınıf ProjectFileInfo"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ProjectFileInfo sınıfı. Sınıf örneği, proje dosyasının formatı ve dosyanın oluşturulduğu Microsoft Project sürümü hakkında bilgi içerir."
type: docs
weight: 1460
url: /tr/net/aspose.tasks/projectfileinfo/
---
## ProjectFileInfo class

Sınıf örneği, dosyanın oluşturulduğu Microsoft Project sürümü ve proje dosya biçimi hakkında bilgi içerir.

```csharp
public sealed class ProjectFileInfo : IEquatable<ProjectFileInfo>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CanRead](../../aspose.tasks/projectfileinfo/canread/) { get; } | Aspose.Tasks'in proje dosyasını işleyip işleyemeyeceğini gösteren bir değeri alır. |
| [IsPasswordProtected](../../aspose.tasks/projectfileinfo/ispasswordprotected/) { get; } | Bir projenin şifre korumalı olup olmadığını gösteren bir değeri alır. |
| [ProjectApplicationInfo](../../aspose.tasks/projectfileinfo/projectapplicationinfo/) { get; } | Proje dosyası uygulama bilgisini alır. |
| [ProjectFileFormat](../../aspose.tasks/projectfileinfo/projectfileformat/) { get; } | Proje dosyası formatını alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [Equals](../../aspose.tasks/projectfileinfo/equals/#equals_1)(object) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| [Equals](../../aspose.tasks/projectfileinfo/equals/#equals)(ProjectFileInfo) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| override [GetHashCode](../../aspose.tasks/projectfileinfo/gethashcode/)() | `ProjectFileInfo` sınıfının örneği için bir karma kod değeri döndürür. |

## Açıklamalar

Kütüphanenin proje dosyasını işleyebileceğini tanımlamak için CanRead özelliğini kullanın.

## Örnekler

Proje dosyası bilgilerini nasıl okuyacağınızı gösterir.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


