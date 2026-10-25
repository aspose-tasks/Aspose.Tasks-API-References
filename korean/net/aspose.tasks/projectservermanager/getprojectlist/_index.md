---
title: "ProjectServerManager.GetProjectList"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProjectServerManager 메서드. 현재 Project Online 계정 및 Project Server 인스턴스의 작업 저장소에서 프로젝트 목록을 가져옵니다."
type: docs
weight: 50
url: /ko/net/aspose.tasks/projectservermanager/getprojectlist/
---
## ProjectServerManager.GetProjectList method

현재 Project Online 계정 \\ Project Server 인스턴스의 'Working' 저장소에서 프로젝트 목록을 가져옵니다.

```csharp
public IEnumerable<ProjectInfo> GetProjectList()
```

### 반환 값

현재 Project Online 계정 \\ Project Server 인스턴스에 있는 프로젝트의 열거형입니다.

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

* class [ProjectInfo](../../projectinfo/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


