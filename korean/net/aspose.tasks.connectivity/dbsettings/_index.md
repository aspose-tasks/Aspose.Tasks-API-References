---
title: "DbSettings 클래스"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Connectivity.DbSettings 클래스. 프로젝트 데이터베이스에서 읽기 위한 설정을 지정할 수 있습니다."
type: docs
weight: 290
url: /ko/net/aspose.tasks.connectivity/dbsettings/
---
## DbSettings class

프로젝트 데이터베이스에서 읽기 위한 설정을 지정할 수 있습니다.

```csharp
public abstract class DbSettings
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | 연결 문자열을 가져오거나 설정합니다. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | 프로젝트 로드 작업 중에 호출될 콜백을 가져오거나 설정합니다. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | DB에 연결하는 데 사용되는 DbProviderFactory 인스턴스를 가져오거나 설정합니다. ProviderFactory와 ProviderInvariantName이 모두 설정된 경우 ProviderFactory가 우선합니다. 기본값은 null입니다. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | DbProviderFactory 클래스의 인스턴스를 가져오는 데 사용되는 provider invariant name을 가져오거나 설정합니다. 기본값은 SqlClient입니다. |

## 예제

프로바이더 이름을 사용하여 여러 프로젝트가 포함된 Primavera XML 파일에서 프로젝트를 읽는 방법을 보여줍니다.

```csharp
var connectionString = "Data Source=" + DataDir + "\\PPMDBSQLite.db";

// 연결 문자열과 프로젝트 ID를 사용하여 Primavera DB 설정 만들기
var settings = new PrimaveraDbSettings(connectionString, 4502);
settings.ProviderInvariantName = "System.Data.SQLite";

Console.WriteLine("Connection String: " + settings.ConnectionString);
Console.WriteLine("Provider Name: " + settings.ProviderInvariantName);

var project = new Project(settings);
project.Save(OutDir + "SupportForSQLiteDatabase_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


