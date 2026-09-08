---
title: "DbSettings.ProviderFactory"
second_title: "Aspose.Tasks for .NET API 참조"
description: "DbSettings 속성. DB에 연결하는 데 사용되는 DbProviderFactory 인스턴스를 가져오거나 설정합니다. ProviderFactory와 ProviderInvariantName이 모두 설정된 경우 ProviderFactory가 우선합니다. 기본값은 null입니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks.connectivity/dbsettings/providerfactory/
---
## DbSettings.ProviderFactory property

DB에 연결하는 데 사용되는 DbProviderFactory 인스턴스를 가져오거나 설정합니다. ProviderFactory와 ProviderInvariantName이 모두 설정된 경우 ProviderFactory가 우선합니다. 기본값은 null입니다.

```csharp
public DbProviderFactory ProviderFactory { get; set; }
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

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


