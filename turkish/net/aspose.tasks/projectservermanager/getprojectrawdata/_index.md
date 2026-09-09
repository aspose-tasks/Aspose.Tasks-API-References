---
title: "ProjectServerManager.GetProjectRawData"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectServerManager yöntemi. Sorun giderme amaçları için projenin ikili verilerini alır."
type: docs
weight: 60
url: /tr/net/aspose.tasks/projectservermanager/getprojectrawdata/
---
## ProjectServerManager.GetProjectRawData method

Sorun giderme amaçları için projenin ikili verilerini alır.

```csharp
public Stream GetProjectRawData(Guid projectGuid)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| projectGuid | Guid | Okunacak projenin Guid'i. |

### Dönüş Değeri

Projenin ham verilerini içeren akış.

## Örnekler

```csharp
In this example the debug info for the specific project is retrieved. You can pass the resulting "debug.zip" to the support team for troubleshooting purposes.
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
// Almaya çalıştığınız projenin guid'i.
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

Microsoft Project Online'dan projenin ham verilerini sorun giderme amaçlarıyla nasıl alacağınızı gösterir.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);
var manager = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = manager.GetProjectList();

foreach (var info in list)
{
    var project = manager.GetProject(info.Id);
    Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
    Console.WriteLine("Resources count: {0}", project.Resources.Count);

    // Kullanıcı, sorunun giderilmesi amacıyla projeyi ham veri akışı olarak okuyabilir.
    using (FileStream fs = File.Create(OutDir + "projectRawData.zip"))
    {
        using (var stream = manager.GetProjectRawData(info.Id))
        {
            stream.CopyTo(fs);
        }
    }

    // Oluşan dosyayı destek birimine gönderebilirsiniz.
}
```

### Ayrıca Bakınız

* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


