---
title: "클래스 ProjectServerCredentials"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ProjectServerCredentials 클래스. Project Online 또는 온프레미스 Project Server 인스턴스에 연결하는 데 사용되는 자격 증명"
type: docs
weight: 1490
url: /ko/net/aspose.tasks/projectservercredentials/
---
## ProjectServerCredentials class

Project Online 또는 온프레미스 Project Server 인스턴스에 연결하는 데 사용되는 자격 증명을 나타냅니다.

```csharp
public sealed class ProjectServerCredentials
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [ProjectServerCredentials](projectservercredentials/#constructor)(string, NetworkCredential) | Project Web Access 엔드포인트 URL과 네트워크 자격 증명을 사용하여 `ProjectServerCredentials` 클래스의 새 인스턴스를 초기화합니다. |
| [ProjectServerCredentials](projectservercredentials/#constructor_1)(string, string) | SharePoint 사이트 URL과 SharePoint의 PWA(프로젝트 웹 액세스) 사이트에 대한 유효한 SPOIDCRL 인증 토큰을 사용하여 `ProjectServerCredentials` 클래스의 새 인스턴스를 초기화합니다. |
| [ProjectServerCredentials](projectservercredentials/#constructor_2)(string, string, string) | SharePoint 사이트 URL, 사용자 이름 및 비밀번호를 사용하여 `ProjectServerCredentials` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [AuthToken](../../aspose.tasks/projectservercredentials/authtoken/) { get; } | SharePoint 인스턴스에 대한 인증 토큰을 가져옵니다. |
| [SiteUrl](../../aspose.tasks/projectservercredentials/siteurl/) { get; } | SharePoint 사이트의 PWA URL 또는 온프레미스 Project Server URL을 가져옵니다. 예: https://your_company_name.sharepoint.com/sites/pwa\"; |
| [UserName](../../aspose.tasks/projectservercredentials/username/) { get; } | SharePoint 사이트의 사용자 이름을 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| override [ToString](../../aspose.tasks/projectservercredentials/tostring/)() | 이 인스턴스의 문자열 표현을 반환합니다. |

## 예제

Microsoft Project Online에서 프로젝트 목록을 검색하기 위해 프로젝트 서버 자격 증명을 사용하는 방법을 보여줍니다.

```csharp
try
{
    const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

    var newProject = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.CreateNewProject(newProject);

    IEnumerable<ProjectInfo> list = manager.GetProjectList();

    foreach (var info in list)
    {
        var project = manager.GetProject(info.Id);
        Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
        Console.WriteLine("Resources count: {0}", project.Resources.Count);
    }
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


