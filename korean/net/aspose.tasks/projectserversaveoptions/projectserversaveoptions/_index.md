---
title: "ProjectServerSaveOptions.ProjectServerSaveOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProjectServerSaveOptions 생성자. ProjectServerSaveOptions 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/projectserversaveoptions/projectserversaveoptions/
---
## ProjectServerSaveOptions constructor

[`ProjectServerSaveOptions`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public ProjectServerSaveOptions()
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


