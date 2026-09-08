---
title: "ProjectServerManager.UpdateProject"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProjectServerManager 메서드. 기본 저장 옵션을 사용하여 Project Server/Project Online 인스턴스의 기존 프로젝트를 업데이트합니다. 기존 프로젝트가 덮어쓰기됩니다."
type: docs
weight: 70
url: /ko/net/aspose.tasks/projectservermanager/updateproject/
---
## UpdateProject(Project) {#updateproject}

기본 저장 옵션을 사용하여 Project Server\\Project Online 인스턴스의 기존 프로젝트를 업데이트합니다. 기존 프로젝트가 덮어쓰기됩니다.

```csharp
public void UpdateProject(Project project)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 프로젝트 | Project | Project Server\Project Online 인스턴스에 저장할 프로젝트. |

### 예외

| 예외 | 조건 |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | 통신 오류가 발생하거나 서버에서 오류가 반환된 경우. |

## 비고

Project의 속성 'project.Get(Prj.Guid)'는 Project Server 계정 \ Project Online 인스턴스에 존재하는 프로젝트의 유효한 GUID여야 합니다.

## 예제

이 예제에서는 프로젝트를 Project Online 계정에서 로드하고, 수정한 뒤 다시 Project Online 계정에 저장합니다.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("New task");
manager.UpdateProject(project);
```

Microsoft Project Online에서 프로젝트를 업데이트하는 방법을 보여줍니다.

```csharp
const string URL = "https://contoso.sharepoint.com/sites/pwa";
const string Domain = "CONTOSO.COM";
const string UserName = "Administrator";
const string Password = "MyPassword";

var windowsCredentials = new NetworkCredential(UserName, Password, Domain);
var projectServerCredentials = new ProjectServerCredentials(URL, windowsCredentials);
try
{
    var manager = new ProjectServerManager(projectServerCredentials);

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

    manager.UpdateProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine("Failed to update the project. Error: " + ex);
}
```

### 또 보기

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## UpdateProject(Project, ProjectServerSaveOptions) {#updateproject_1}

지정된 저장 옵션을 사용하여 Project Server\\Project Online 인스턴스의 기존 프로젝트를 업데이트합니다. 기존 프로젝트가 덮어쓰기됩니다.

```csharp
public void UpdateProject(Project project, ProjectServerSaveOptions saveOptions)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 프로젝트 | Project | Project Server\Project Online 인스턴스에 저장할 프로젝트. |
| saveOptions | ProjectServerSaveOptions | [`ProjectServerSaveOptions`](../../projectserversaveoptions/) 클래스의 인스턴스. |

### 예외

| 예외 | 조건 |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | 통신 오류가 발생하거나 서버에서 오류가 반환된 경우. |

## 비고

saveOptions.ProjectGuid는 Project Server\ Project Online 인스턴스에 존재하는 프로젝트의 GUID로 설정되어야 합니다.

## 예제

이 예제에서는 프로젝트를 Project Online 계정에서 로드하고, 수정한 뒤 다시 Project Online 계정에 저장합니다.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("New task");
manager.UpdateProject(project, new ProjectServerSaveOptions
{
    ProjectGuid = projectGuid
});
```

Project Server 저장 옵션을 사용하여 Microsoft Project Online에서 프로젝트를 업데이트하는 방법을 보여줍니다.

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

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


