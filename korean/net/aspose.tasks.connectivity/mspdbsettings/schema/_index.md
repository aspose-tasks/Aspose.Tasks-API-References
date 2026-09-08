---
title: "MspDbSettings.Schema"
second_title: "Aspose.Tasks for .NET API 참조"
description: "MspDbSettings 속성. MS Project Server의 스키마를 가져오거나 설정합니다. 기본값은 pub입니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks.connectivity/mspdbsettings/schema/
---
## MspDbSettings.Schema property

MS Project Server의 스키마를 가져오거나 설정합니다. 기본값은 "pub"입니다.

```csharp
public string Schema { get; set; }
```

## 예제

데이터베이스에서 프로젝트를 가져오는 방법을 보여줍니다.

```csharp
try
{
    // 연결 문자열 만들기
    var connectionString = new SqlConnectionStringBuilder();
    connectionString.DataSource = "192.168.56.2,1433";
    connectionString.Encrypt = true;
    connectionString.TrustServerCertificate = true;
    connectionString.InitialCatalog = "ProjectServer_Published";
    connectionString.NetworkLibrary = "DBMSSOCN";
    connectionString.UserID = "sa";
    connectionString.Password = "*****";

    // MS 데이터베이스에서 로드하기 위한 설정 만들기
    var settings = new MspDbSettings(connectionString.ConnectionString, new Guid("E6426C44-D6CB-4B9C-AF16-48910ACE0F54"));
    settings.Schema = "dbo";

    Console.WriteLine("Project GUID to load: " + settings.ProjectGuid);

    var project = new Project(settings);

    project.Save(OutDir + "ImportProjectDataFromDatabase_out.mpp", SaveFileFormat.Mpp);
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message + " Please setup proper data source (DataSource, InitialCatalog etc)");
}
```

### 또 보기

* class [MspDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mspdbsettings/)
* assembly [Aspose.Tasks](../../../)


