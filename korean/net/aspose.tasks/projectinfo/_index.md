---
title: "클래스 ProjectInfo"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ProjectInfo 클래스. Project Online에서 사용할 수 있는 게시된 프로젝트에 대한 간략한 정보"
type: docs
weight: 1470
url: /ko/net/aspose.tasks/projectinfo/
---
## ProjectInfo class

Project Online에서 사용할 수 있는 게시된 프로젝트에 대한 간략한 정보입니다.

```csharp
public sealed class ProjectInfo
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [ProjectInfo](projectinfo/)() | `ProjectInfo` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [CreatedDate](../../aspose.tasks/projectinfo/createddate/) { get; } | 프로젝트가 생성된 날짜와 시간을 가져옵니다. |
| [Description](../../aspose.tasks/projectinfo/description/) { get; } | 프로젝트의 설명을 가져옵니다. |
| [Id](../../aspose.tasks/projectinfo/id/) { get; } | 프로젝트의 고유 식별자를 가져옵니다. |
| [IsCheckedOut](../../aspose.tasks/projectinfo/ischeckedout/) { get; } | 프로젝트가 체크아웃 되었는지 여부를 나타내는 값을 가져옵니다. |
| [LastPublishedDate](../../aspose.tasks/projectinfo/lastpublisheddate/) { get; } | 프로젝트가 가장 최근에 게시된 날짜를 가져옵니다. |
| [LastSavedDate](../../aspose.tasks/projectinfo/lastsaveddate/) { get; } | 프로젝트가 가장 최근에 저장된 날짜를 가져옵니다. |
| [Name](../../aspose.tasks/projectinfo/name/) { get; } | 프로젝트의 이름을 가져옵니다. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


