---
title: "ProjectServerSaveOptions.ProjectServerSaveOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectServerSaveOptions yapıcı. ProjectServerSaveOptions sınıfının yeni bir örneğini başlatır"
type: docs
weight: 10
url: /tr/net/aspose.tasks/projectserversaveoptions/projectserversaveoptions/
---
## ProjectServerSaveOptions constructor

[`ProjectServerSaveOptions`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public ProjectServerSaveOptions()
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


