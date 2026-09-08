---
title: "ProjectServerManager.GetProjectRawData"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProjectServerManager 메서드. 문제 해결을 위해 프로젝트의 바이너리 데이터를 가져옵니다."
type: docs
weight: 60
url: /ko/net/aspose.tasks/projectservermanager/getprojectrawdata/
---
## ProjectServerManager.GetProjectRawData method

문제 해결을 위해 프로젝트의 바이너리 데이터를 가져옵니다.

```csharp
public Stream GetProjectRawData(Guid projectGuid)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| projectGuid | Guid | 읽을 프로젝트의 Guid입니다. |

### 반환 값

프로젝트 원시 데이터를 포함하는 스트림.

## 예제

```csharp
In this example the debug info for the specific project is retrieved. You can pass the resulting "debug.zip" to the support team for troubleshooting purposes.
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
// 가져오려는 프로젝트의 GUID.
var projectGuid = new Guid("e0294bfb-5657-45c8-9cc5-82169fb95d69");
ProjectServerManager manager = new ProjectServerManager(credentials);
using (var fileStream = File.OpenWrite(@"c:\debug.zip"))
{
    using (var stream = manager.GetProjectRawData(projectGuid))
    {
        stream.CopyTo(fileStream);
    }
}
```

문제 해결을 위해 Microsoft Project Online에서 프로젝트의 원시 데이터를 검색하는 방법을 보여줍니다.

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

    // 사용자는 문제 해결을 위해 프로젝트를 원시 데이터 스트림으로 읽을 수 있습니다.
    using (FileStream fs = File.Create(OutDir + "projectRawData.zip"))
    {
        using (var stream = manager.GetProjectRawData(info.Id))
        {
            stream.CopyTo(fs);
        }
    }

    // 결과 파일을 지원팀에 전달할 수 있습니다.
}
```

### 또 보기

* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


