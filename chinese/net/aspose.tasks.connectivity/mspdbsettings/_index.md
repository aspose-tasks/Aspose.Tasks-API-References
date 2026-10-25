---
title: "类 MspDbSettings"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Connectivity.MspDbSettings 类。允许设置读取来自 MS Project Server 数据库的项目数据所需的选项"
type: docs
weight: 310
url: /zh/net/aspose.tasks.connectivity/mspdbsettings/
---
## MspDbSettings class

允许设置必要的选项以从 MS Project Server 数据库读取项目数据。

```csharp
public class MspDbSettings : DbSettings
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [MspDbSettings](mspdbsettings/)(string, Guid) | 初始化 `MspDbSettings` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | 获取或设置连接字符串。 |
| [ProjectGuid](../../aspose.tasks.connectivity/mspdbsettings/projectguid/) { get; } | 获取要读取的项目的 guid。 |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | 获取或设置在项目加载操作期间调用的回调函数。 |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | 获取或设置用于连接数据库的 DbProviderFactory 实例。如果同时设置了 ProviderFactory 和 ProviderInvariantName，则 ProviderFactory 优先。默认值为 null。 |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | 获取或设置用于获取 DbProviderFactory 类实例的提供程序不变名称。默认值为 SqlClient。 |
| [Schema](../../aspose.tasks.connectivity/mspdbsettings/schema/) { get; set; } | 获取或设置 MS Project Server 的模式。默认值为 "pub"。 |

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

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


