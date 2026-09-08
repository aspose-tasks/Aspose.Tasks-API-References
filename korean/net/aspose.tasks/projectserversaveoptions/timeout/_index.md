---
title: "ProjectServerSaveOptions.Timeout"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProjectServerSaveOptions 속성. Project Server의 큐 처리 서비스가 저장 프로젝트 요청을 처리할 때 대기하는 데 사용되는 시간 제한을 가져오거나 설정합니다. 이 속성의 기본값은 1분입니다."
type: docs
weight: 50
url: /ko/net/aspose.tasks/projectserversaveoptions/timeout/
---
## ProjectServerSaveOptions.Timeout property

Project Server의 큐 처리 서비스가 프로젝트 저장 요청을 처리할 때 대기하는 데 사용되는 시간 제한을 가져오거나 설정합니다. 이 속성의 기본값은 1분입니다.

```csharp
public TimeSpan Timeout { get; set; }
```

## 비고

프로젝트가 크거나 Project Server 인스턴스가 다른 요청에 응답하느라 너무 바쁠 경우 처리 시간이 더 길어질 수 있습니다.

## 예제

Microsoft Project Online에서 프로젝트를 업데이트하고 저장 시간 제한 값을 제어하는 방법을 보여줍니다.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);
try
{
    var manager = new ProjectServerManager(credentials);

    ProjectInfo projectInfo = null;
    foreach (var info in manager.GetProjectList())
    {
        if (info.Name == "My project")
        {
            projectInfo = info;
        }
    }

    if (projectInfo == null)
    {
        Console.WriteLine("Project 'My project' not found in working store of Project Online account.");
        return;
    }

    var project = manager.GetProject(projectInfo.Id);
    project.Set(Prj.FinishDate, new DateTime(2020, 03, 01));

    var task = project.RootTask.Children.Add("New task");
    task.Set(Tsk.Start, new DateTime(2020, 02, 26));
    task.Set(Tsk.Duration, project.GetDuration(2, TimeUnitType.Day));

    var options = new ProjectServerSaveOptions { Timeout = TimeSpan.FromMinutes(5) };

    manager.UpdateProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine("Failed to update the project. Error: " + ex);
}
```

### 또 보기

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


