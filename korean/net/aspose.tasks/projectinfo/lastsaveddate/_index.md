---
title: "ProjectInfo.LastSavedDate"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProjectInfo 속성. 프로젝트가 마지막으로 저장된 최신 날짜를 가져옵니다."
type: docs
weight: 70
url: /ko/net/aspose.tasks/projectinfo/lastsaveddate/
---
## ProjectInfo.LastSavedDate property

프로젝트가 가장 최근에 저장된 날짜를 가져옵니다.

```csharp
public DateTime LastSavedDate { get; }
```

## 예제

Project Online에서 프로젝트 정보를 읽는 방법을 보여줍니다.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

var reader = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = reader.GetProjectList();

// 프로젝트 정보를 읽습니다
Console.WriteLine("Print information about projects:");
foreach (var info in list)
{
    Console.WriteLine("Id: " + info.Id);
    Console.WriteLine("Name: " + info.Name);
    Console.WriteLine("Description: " + info.Description);
    Console.WriteLine("Created Date: " + info.CreatedDate);
    Console.WriteLine("Last Saved Date: " + info.LastSavedDate);
    Console.WriteLine("Last Published Date: " + info.LastPublishedDate);
    Console.WriteLine("Is Checked Out: " + info.IsCheckedOut);
}
```

### 또 보기

* class [ProjectInfo](../)
* namespace [Aspose.Tasks](../../projectinfo/)
* assembly [Aspose.Tasks](../../../)


