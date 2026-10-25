---
title: "ProjectServerSaveOptions.PollingInterval"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProjectServerSaveOptions 속성. 큐 작업 상태 요청 사이의 간격을 가져오거나 설정합니다. 기본값은 2초입니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks/projectserversaveoptions/pollinginterval/
---
## ProjectServerSaveOptions.PollingInterval property

큐 작업 상태 요청 사이의 간격을 가져오거나 설정합니다. 기본값은 2초입니다.

```csharp
public TimeSpan PollingInterval { get; set; }
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


