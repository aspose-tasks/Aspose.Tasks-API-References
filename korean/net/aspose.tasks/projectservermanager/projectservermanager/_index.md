---
title: "ProjectServerManager.ProjectServerManager"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProjectServerManager 생성자. ProjectServerManager 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/projectservermanager/projectservermanager/
---
## ProjectServerManager constructor

[`ProjectServerManager`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public ProjectServerManager(ProjectServerCredentials credentials)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 자격 증명 | ProjectServerCredentials | Project Online 계정에 연결하는 데 사용되는 자격 증명. |

## 예제

이 예제는 ProjectServerManager 인스턴스를 생성하여 온프레미스 Project Server 인스턴스에 액세스하는 방법을 보여줍니다.

```csharp
[C#]
string site = "http://project_server_instance.local/";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

이 예제는 ProjectServerManager 인스턴스를 생성하여 Project Online 서비스의 계정에 액세스하는 방법을 보여줍니다.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

Microsoft Project Online에서 프로젝트를 읽는 방법을 보여줍니다.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);
var manager = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = manager.GetProjectList();

foreach (var info in list)
{
    var project = manager.GetProject(info.Id);
    Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
    Console.WriteLine("Resources count: {0}", project.Resources.Count);
}
```

### 또 보기

* class [ProjectServerCredentials](../../projectservercredentials/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


