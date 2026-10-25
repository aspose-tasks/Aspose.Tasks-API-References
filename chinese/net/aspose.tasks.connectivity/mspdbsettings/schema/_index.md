---
title: "MspDbSettings.Schema"
second_title: "Aspose.Tasks for .NET API 参考"
description: "MspDbSettings 属性。获取或设置 MS Project Server 的模式。默认值为 pub"
type: docs
weight: 30
url: /zh/net/aspose.tasks.connectivity/mspdbsettings/schema/
---
## MspDbSettings.Schema property

获取或设置 MS Project Server 的模式。默认值为 "pub"。

```csharp
public string Schema { get; set; }
```

## 示例

展示如何从数据库导入项目。

```csharp
try
{
    // 创建连接字符串
    var connectionString = new SqlConnectionStringBuilder();
    connectionString.DataSource = "192.168.56.2,1433";
    connectionString.Encrypt = true;
    connectionString.TrustServerCertificate = true;
    connectionString.InitialCatalog = "ProjectServer_Published";
    connectionString.NetworkLibrary = "DBMSSOCN";
    connectionString.UserID = "sa";
    connectionString.Password = "*****";

    // 创建用于从 MS 数据库加载的设置
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

### 另见

* class [MspDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mspdbsettings/)
* assembly [Aspose.Tasks](../../../)


