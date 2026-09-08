---
title: "클래스 ProjectServerManager"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ProjectServerManager 클래스. 지정된 Project Online 계정 또는 지정된 온프레미스 Project Server 인스턴스의 프로젝트를 읽고 작업을 수행하는 메서드를 제공하는 클래스이며, Project Server 버전 2016 및 2019를 지원합니다."
type: docs
weight: 1500
url: /ko/net/aspose.tasks/projectservermanager/
---
## ProjectServerManager class

지정된 Project Online 계정 또는 지정된 온프레미스 Project Server 인스턴스(지원되는 Project Server 버전은 2016 및 2019)에서 프로젝트를 읽고 작업을 수행하는 메서드를 제공하는 클래스입니다.

```csharp
public sealed class ProjectServerManager
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [ProjectServerManager](projectservermanager/)(ProjectServerCredentials) | `ProjectServerManager` 클래스의 새 인스턴스를 초기화합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject)(Project) | 기본 저장 옵션을 사용하여 Project Server\Project Online 인스턴스에 새 프로젝트를 생성합니다. |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject_1)(Project, ProjectServerSaveOptions) | 지정된 저장 옵션을 사용하여 Project Server\\Project Online 인스턴스에 새 프로젝트를 생성합니다. |
| [GetProject](../../aspose.tasks/projectservermanager/getproject/)(Guid) | Project Online 계정 \\ Project Server 인스턴스에서 지정된 GUID를 가진 프로젝트를 가져옵니다. |
| [GetProjectList](../../aspose.tasks/projectservermanager/getprojectlist/)() | 현재 Project Online 계정 \\ Project Server 인스턴스의 'Working' 저장소에서 프로젝트 목록을 가져옵니다. |
| [GetProjectRawData](../../aspose.tasks/projectservermanager/getprojectrawdata/)(Guid) | 문제 해결을 위해 프로젝트의 바이너리 데이터를 가져옵니다. |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject)(Project) | 기본 저장 옵션을 사용하여 Project Server\\Project Online 인스턴스의 기존 프로젝트를 업데이트합니다. 기존 프로젝트가 덮어쓰기됩니다. |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject_1)(Project, ProjectServerSaveOptions) | 지정된 저장 옵션을 사용하여 Project Server\\Project Online 인스턴스의 기존 프로젝트를 업데이트합니다. 기존 프로젝트가 덮어쓰기됩니다. |

## 이벤트

| 이름 | 설명 |
| --- | --- |
| event [ExecutingWebRequest](../../aspose.tasks/projectservermanager/executingwebrequest/) | 웹 요청이 Project Server의 웹 API로 전송될 때 발생하는 이벤트입니다. |

## 예제

Microsoft Project Online에서 미리 정의된 저장 옵션으로 새 프로젝트를 만들기 위해 Project Server 관리자를 사용하는 방법을 보여줍니다.

```csharp
try
{
    const string sharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(sharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    var options = new ProjectServerSaveOptions
    {
        Timeout = TimeSpan.FromSeconds(10)
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


