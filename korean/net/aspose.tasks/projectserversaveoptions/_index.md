---
title: "클래스 ProjectServerSaveOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ProjectServerSaveOptions 클래스. 프로젝트를 Project Server 또는 Project Online에 저장할 때 추가 옵션을 지정할 수 있습니다."
type: docs
weight: 1510
url: /ko/net/aspose.tasks/projectserversaveoptions/
---
## ProjectServerSaveOptions class

프로젝트를 Project Server 또는 Project Online에 저장할 때 추가 옵션을 지정할 수 있습니다.

```csharp
public sealed class ProjectServerSaveOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [ProjectServerSaveOptions](projectserversaveoptions/)() | 새 `ProjectServerSaveOptions` 클래스의 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [PollingInterval](../../aspose.tasks/projectserversaveoptions/pollinginterval/) { get; set; } | 큐 작업 상태 요청 사이의 간격을 가져오거나 설정합니다. 기본값은 2초입니다. |
| [ProjectGuid](../../aspose.tasks/projectserversaveoptions/projectguid/) { get; set; } | 프로젝트의 고유 식별자를 가져오거나 설정합니다. Project Server \\ Project Online 인스턴스 내에서 고유해야 합니다. |
| [ProjectName](../../aspose.tasks/projectserversaveoptions/projectname/) { get; set; } | Project Server \\ Project Online 프로젝트 목록에 표시되는 프로젝트 이름을 가져오거나 설정합니다. Project Server \\ Project Online 인스턴스 내에서 고유해야 합니다. 값이 생략된 경우, 대신 Prj.Name 속성의 값이 사용됩니다. |
| [Timeout](../../aspose.tasks/projectserversaveoptions/timeout/) { get; set; } | Project Server의 큐 처리 서비스가 프로젝트 저장 요청을 처리할 때 대기하는 데 사용되는 시간 제한을 가져오거나 설정합니다. 이 속성의 기본값은 1분입니다. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


