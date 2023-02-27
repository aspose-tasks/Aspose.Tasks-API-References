---
title: ProjectServerManager.GetProjectRawData
second_title: Aspose.Tasks for .NET API Referansı
description: ProjectServerManager yöntem. Sorun giderme amacıyla projenin ikili verilerini alır.
type: docs
weight: 60
url: /tr/net/aspose.tasks/projectservermanager/getprojectrawdata/
---
## ProjectServerManager.GetProjectRawData method

Sorun giderme amacıyla projenin ikili verilerini alır.

```csharp
public Stream GetProjectRawData(Guid projectGuid)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| projectGuid | Guid | Okumak için projenin Rehberi. |

### Geri dönüş değeri

Ham projenin verilerini içeren akış.

### Örnekler

```csharp
In this example the debug info for the specific project is retrieved. You can pass the resulting "debug.zip" to the support team for troubleshooting purposes.
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "şifre");
// Almaya çalıştığınız projenin rehberi.
var projectGuid = new Guid("e0294bfb-5657-45c8-9cc5-82169fb95d69");
ProjectServerManager manager = new ProjectServerManager(credentials);
using (var fileStream = File.OpenWrite(@"c:\debug.zip"))
{
    using (var stream = manager.GetProjectRawData(projectGuid))
    {
        stream.CopyTo(fileStream);
    }
}
```

### Ayrıca bakınız

* class [ProjectServerManager](../)
* ad alanı [Aspose.Tasks](../../projectservermanager/)
* toplantı [Aspose.Tasks](../../../)


