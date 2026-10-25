---
title: "ProjectServerManager.GetProject"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProjectServerManager 메서드. 지정된 guid를 사용하여 Project Online 계정의 Project Server 인스턴스에서 프로젝트를 가져옵니다"
type: docs
weight: 40
url: /ko/net/aspose.tasks/projectservermanager/getproject/
---
## ProjectServerManager.GetProject method

Project Online 계정 \\ Project Server 인스턴스에서 지정된 GUID를 가진 프로젝트를 가져옵니다.

```csharp
public Project GetProject(Guid projectGuid)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| projectGuid | Guid | 읽을 프로젝트의 Guid입니다. |

### 반환 값

[`Project`](../../project/) 클래스의 인스턴스로, Project Online \\ Project Server에서 읽은 프로젝트를 나타냅니다.

## 예제

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

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


