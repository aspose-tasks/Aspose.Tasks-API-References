---
title: "PrimaveraDbSettings.PrimaveraDbSettings"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PrimaveraDbSettings 생성자. PrimaveraDbSettings 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.connectivity/primaveradbsettings/primaveradbsettings/
---
## PrimaveraDbSettings constructor

새 인스턴스를 초기화합니다. [`PrimaveraDbSettings`](../) 클래스.

```csharp
public PrimaveraDbSettings(string connectionString, int projectId)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| connectionString | 문자열 | 지정된 연결 문자열입니다. |
| projectId | Int32 | 읽을 프로젝트의 지정된 ID입니다. |

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


