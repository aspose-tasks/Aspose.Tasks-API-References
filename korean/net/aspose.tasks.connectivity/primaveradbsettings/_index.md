---
title: "PrimaveraDbSettings 클래스"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Connectivity.PrimaveraDbSettings 클래스. Primavera 데이터베이스에서 프로젝트 데이터를 읽기 위해 필요한 옵션을 설정할 수 있습니다."
type: docs
weight: 320
url: /ko/net/aspose.tasks.connectivity/primaveradbsettings/
---
## PrimaveraDbSettings class

Primavera 데이터베이스에서 프로젝트 데이터를 읽기 위한 필요한 옵션을 설정할 수 있습니다.

```csharp
public class PrimaveraDbSettings : DbSettings
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [PrimaveraDbSettings](primaveradbsettings/)(string, int) | `PrimaveraDbSettings` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | 연결 문자열을 가져오거나 설정합니다. |
| [ProjectId](../../aspose.tasks.connectivity/primaveradbsettings/projectid/) { get; } | 읽을 프로젝트의 ID를 가져옵니다. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | 프로젝트 로드 작업 중에 호출될 콜백을 가져오거나 설정합니다. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | DB에 연결하는 데 사용되는 DbProviderFactory 인스턴스를 가져오거나 설정합니다. ProviderFactory와 ProviderInvariantName이 모두 설정된 경우 ProviderFactory가 우선합니다. 기본값은 null입니다. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | DbProviderFactory 클래스의 인스턴스를 가져오는 데 사용되는 provider invariant name을 가져오거나 설정합니다. 기본값은 SqlClient입니다. |

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

Primavera 데이터베이스에서 프로젝트의 간략 정보를 가져오는 방법을 보여줍니다.

```csharp
var settings = new PrimaveraDbSettings(GetConnectionString(), 0);

var reader = new PrimaveraDbReader(settings);
var projectInfos = reader.GetProjectInfos();

foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - '{2}'", info.Uid, info.ShortName, info.Name);
}

var firstProject = reader.LoadProject(projectInfos[0].Uid);
Console.WriteLine(firstProject.Uid);
Console.WriteLine(firstProject.Name);
Console.WriteLine(firstProject.PrimaveraProperties.ShortName);
```

### 또 보기

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


