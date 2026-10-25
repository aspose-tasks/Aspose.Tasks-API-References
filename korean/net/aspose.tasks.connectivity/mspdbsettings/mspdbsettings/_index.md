---
title: "MspDbSettings.MspDbSettings"
second_title: "Aspose.Tasks for .NET API 참조"
description: "MspDbSettings 생성자. MspDbSettings 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.connectivity/mspdbsettings/mspdbsettings/
---
## MspDbSettings constructor

새 인스턴스를 초기화합니다. [`MspDbSettings`](../) 클래스.

```csharp
public MspDbSettings(string connectionString, Guid projectGuid)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| connectionString | 문자열 | 지정된 연결 문자열입니다. |
| projectGuid | Guid | 읽을 프로젝트의 지정된 GUID입니다. |

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


