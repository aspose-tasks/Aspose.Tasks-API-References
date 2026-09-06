---
title: "MspDbSettings.MspDbSettings"
second_title: "Aspose.Tasks for .NET API 参考"
description: "MspDbSettings 构造函数。初始化 MspDbSettings 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks.connectivity/mspdbsettings/mspdbsettings/
---
## MspDbSettings constructor

初始化 [`MspDbSettings`](../) 类的新实例。

```csharp
public MspDbSettings(string connectionString, Guid projectGuid)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| connectionString | 字符串 | 指定的连接字符串。 |
| projectGuid | Guid | 指定的要读取的项目 GUID。 |

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


