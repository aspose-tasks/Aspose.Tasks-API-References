---
title: "DbSettings.ConnectionString"
second_title: "Aspose.Tasks for .NET API 참조"
description: "DbSettings 속성. 연결 문자열을 가져오거나 설정합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.connectivity/dbsettings/connectionstring/
---
## DbSettings.ConnectionString property

연결 문자열을 가져오거나 설정합니다.

```csharp
public string ConnectionString { get; set; }
```

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

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


