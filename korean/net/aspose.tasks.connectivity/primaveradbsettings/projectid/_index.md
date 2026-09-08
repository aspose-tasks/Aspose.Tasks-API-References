---
title: "PrimaveraDbSettings.ProjectId"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PrimaveraDbSettings 속성. 읽을 프로젝트의 ID를 가져옵니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks.connectivity/primaveradbsettings/projectid/
---
## PrimaveraDbSettings.ProjectId property

읽을 프로젝트의 ID를 가져옵니다.

```csharp
public int ProjectId { get; }
```

## 예제

Primavera 데이터베이스에서 프로젝트를 가져오는 방법을 보여줍니다.

```csharp
// 연결 문자열과 프로젝트 ID를 사용하여 PrimaveraDbSettings 클래스의 새 인스턴스를 초기화합니다.
var settings = new PrimaveraDbSettings(GetConnectionString(), 4502);
settings.ProviderFactory = SqliteFactory.Instance;

Console.WriteLine("Project UID to read: " + settings.ProjectId);

// UID = 4502인 프로젝트를 읽습니다
var project = new Project(settings);
Console.WriteLine(project.Uid);
Console.WriteLine(project.Name);
Console.WriteLine(project.PrimaveraProperties.ShortName);
```

### 또 보기

* class [PrimaveraDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../primaveradbsettings/)
* assembly [Aspose.Tasks](../../../)


