---
title: "ProjectServerSaveOptions.ProjectGuid"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectServerSaveOptions özelliği. Bir projenin benzersiz tanımlayıcısını alır veya ayarlar. Project Server Project Online örneği içinde benzersiz olmalıdır."
type: docs
weight: 30
url: /tr/net/aspose.tasks/projectserversaveoptions/projectguid/
---
## ProjectServerSaveOptions.ProjectGuid property

Bir projenin benzersiz tanımlayıcısını alır veya ayarlar. Project Server \\ Project Online örneği içinde benzersiz olmalıdır.

```csharp
public Guid ProjectGuid { get; set; }
```

## Örnekler

Yerel (on-premise) Project Server örneğinde yeni bir proje oluşturmak için &lt;see cref=\"Aspose.Tasks.ProjectServerSaveOptions\" /&gt; seçeneklerinin nasıl kullanılacağını gösterir.

```csharp
try
{
    const string URL = "https://project_server.local/sites/pwa";
    const string Domain = "CONTOSO.COM";
    const string UserName = "Administrator";
    const string Password = "MyPassword";

    var project = new Project(DataDir + @"Project1.mpp");

    var windowsCredentials = new NetworkCredential(UserName, Password, Domain);
    var projectServerCredentials = new ProjectServerCredentials(URL, windowsCredentials);
    var manager = new ProjectServerManager(projectServerCredentials);
    var options = new ProjectServerSaveOptions
                      {
                          ProjectGuid = Guid.NewGuid(),
                          ProjectName = "New project",
                          Timeout = TimeSpan.FromMinutes(5),
                          PollingInterval = TimeSpan.FromSeconds(3)
                      };

    manager.CreateNewProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Ayrıca Bakınız

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


