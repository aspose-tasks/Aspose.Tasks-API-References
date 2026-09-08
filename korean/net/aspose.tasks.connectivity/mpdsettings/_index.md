---
title: "MpdSettings 클래스"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Connectivity.MpdSettings 클래스. MPD 형식 MS Access 데이터베이스 파일에서 프로젝트 데이터를 읽기 위해 필요한 옵션을 설정할 수 있습니다."
type: docs
weight: 300
url: /ko/net/aspose.tasks.connectivity/mpdsettings/
---
## MpdSettings class

MPD 형식(MS Access 데이터베이스 파일 형식)에서 프로젝트 데이터를 읽기 위한 필요한 옵션을 설정할 수 있습니다.

```csharp
public class MpdSettings : DbSettings
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [MpdSettings](mpdsettings/)(string, int) | `MpdSettings` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | 연결 문자열을 가져오거나 설정합니다. |
| [ProjectId](../../aspose.tasks.connectivity/mpdsettings/projectid/) { get; } | 읽을 프로젝트의 ID를 가져옵니다. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | 프로젝트 로드 작업 중에 호출될 콜백을 가져오거나 설정합니다. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | DB에 연결하는 데 사용되는 DbProviderFactory 인스턴스를 가져오거나 설정합니다. ProviderFactory와 ProviderInvariantName이 모두 설정된 경우 ProviderFactory가 우선합니다. 기본값은 null입니다. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | DbProviderFactory 클래스의 인스턴스를 가져오는 데 사용되는 provider invariant name을 가져오거나 설정합니다. 기본값은 SqlClient입니다. |

## 예제

데이터베이스에서 프로젝트를 가져오는 것을 제어하기 위해 MPD 설정을 사용하는 방법을 보여줍니다.

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### 또 보기

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


