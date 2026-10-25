---
title: "MpdSettings.ProjectId"
second_title: "Aspose.Tasks for .NET API 참조"
description: "MpdSettings 속성. 읽을 프로젝트의 ID를 가져옵니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks.connectivity/mpdsettings/projectid/
---
## MpdSettings.ProjectId property

읽을 프로젝트의 ID를 가져옵니다.

```csharp
public int ProjectId { get; }
```

## 예제

데이터베이스에서 프로젝트를 가져오는 것을 제어하기 위해 MPD 설정을 사용하는 방법을 보여줍니다.

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### 또 보기

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


