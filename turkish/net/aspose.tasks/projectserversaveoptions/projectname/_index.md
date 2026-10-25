---
title: "ProjectServerSaveOptions.ProjectName"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectServerSaveOptions özelliği. Project Server Project Online projeler listesinde görüntülenen bir projenin adını alır veya ayarlar. Project Server Project Online örneği içinde benzersiz olmalıdır. Değer atlanırsa, Prj.Name özelliğinin değeri kullanılacaktır."
type: docs
weight: 40
url: /tr/net/aspose.tasks/projectserversaveoptions/projectname/
---
## ProjectServerSaveOptions.ProjectName property

Project Server \\ Project Online projeler listesinde görüntülenen bir projenin adını alır veya ayarlar. Project Server \\ Project Online örneği içinde benzersiz olmalıdır. Değer atlanırsa, Prj.Name özelliğinin değeri kullanılacaktır.

```csharp
public string ProjectName { get; set; }
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


