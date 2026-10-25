---
title: "클래스 MspDbSettings"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Connectivity.MspDbSettings 클래스. MS Project Server 데이터베이스에서 프로젝트 데이터를 읽기 위해 필요한 옵션을 설정할 수 있습니다."
type: docs
weight: 310
url: /ko/net/aspose.tasks.connectivity/mspdbsettings/
---
## MspDbSettings class

MS Project Server 데이터베이스에서 프로젝트 데이터를 읽기 위한 필요한 옵션을 설정할 수 있습니다.

```csharp
public class MspDbSettings : DbSettings
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [MspDbSettings](mspdbsettings/)(string, Guid) | `MspDbSettings` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | 연결 문자열을 가져오거나 설정합니다. |
| [ProjectGuid](../../aspose.tasks.connectivity/mspdbsettings/projectguid/) { get; } | 읽을 프로젝트의 GUID를 가져옵니다. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | 프로젝트 로드 작업 중에 호출될 콜백을 가져오거나 설정합니다. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | DB에 연결하는 데 사용되는 DbProviderFactory 인스턴스를 가져오거나 설정합니다. ProviderFactory와 ProviderInvariantName이 모두 설정된 경우 ProviderFactory가 우선합니다. 기본값은 null입니다. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | DbProviderFactory 클래스의 인스턴스를 가져오는 데 사용되는 provider invariant name을 가져오거나 설정합니다. 기본값은 SqlClient입니다. |
| [Schema](../../aspose.tasks.connectivity/mspdbsettings/schema/) { get; set; } | MS Project Server의 스키마를 가져오거나 설정합니다. 기본값은 "pub"입니다. |

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

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


