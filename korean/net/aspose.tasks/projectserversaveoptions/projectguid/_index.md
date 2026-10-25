---
title: "ProjectServerSaveOptions.ProjectGuid"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProjectServerSaveOptions 속성. 프로젝트의 고유 식별자를 가져오거나 설정합니다. Project Server Project Online 인스턴스 내에서 고유해야 합니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks/projectserversaveoptions/projectguid/
---
## ProjectServerSaveOptions.ProjectGuid property

프로젝트의 고유 식별자를 가져오거나 설정합니다. Project Server \\ Project Online 인스턴스 내에서 고유해야 합니다.

```csharp
public Guid ProjectGuid { get; set; }
```

## 예제

온프레미스 Project Server 인스턴스에서 새 프로젝트를 만들기 위해 &lt;see cref=\"Aspose.Tasks.ProjectServerSaveOptions\" /&gt; 옵션을 사용하는 방법을 보여줍니다.

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

### 또 보기

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


