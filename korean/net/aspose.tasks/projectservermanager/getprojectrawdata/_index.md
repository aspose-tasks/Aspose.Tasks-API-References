---
title: GetProjectRawData
second_title: .NET API 참조용 Aspose.Tasks
description: 문제 해결을 위해 프로젝트의 바이너리 데이터를 가져옵니다.
type: docs
weight: 60
url: /ko/net/aspose.tasks/projectservermanager/getprojectrawdata/
---
## ProjectServerManager.GetProjectRawData method

문제 해결을 위해 프로젝트의 바이너리 데이터를 가져옵니다.

```csharp
public Stream GetProjectRawData(Guid projectGuid)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| projectGuid | Guid | 읽을 프로젝트의 Guid입니다. |

### 반환 값

원시 프로젝트의 데이터를 포함하는 스트림.

### 예

```csharp
In this example the debug info for the specific project is retrieved. You can pass the resulting "debug.zip" to the support team for troubleshooting purposes.
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "암호");
// 가져오려는 프로젝트의 가이드입니다.
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

### 또한보십시오

* class [ProjectServerManager](../)
* 네임스페이스 [Aspose.Tasks](../../projectservermanager/)
* 집회 [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
