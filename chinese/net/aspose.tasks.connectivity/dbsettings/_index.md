---
title: "类 DbSettings"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Connectivity.DbSettings 类。允许指定读取项目数据库的设置"
type: docs
weight: 290
url: /zh/net/aspose.tasks.connectivity/dbsettings/
---
## DbSettings class

允许指定从项目数据库读取的设置。

```csharp
public abstract class DbSettings
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | 获取或设置连接字符串。 |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | 获取或设置在项目加载操作期间调用的回调函数。 |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | 获取或设置用于连接数据库的 DbProviderFactory 实例。如果同时设置了 ProviderFactory 和 ProviderInvariantName，则 ProviderFactory 优先。默认值为 null。 |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | 获取或设置用于获取 DbProviderFactory 类实例的提供程序不变名称。默认值为 SqlClient。 |

## 示例

展示如何通过使用提供程序名称从包含多个项目的 Primavera XML 文件读取项目。

```csharp
var connectionString = "Data Source=" + DataDir + "\\PPMDBSQLite.db";

// 使用连接字符串和项目 id 创建 Primavera 数据库设置
var settings = new PrimaveraDbSettings(connectionString, 4502);
settings.ProviderInvariantName = "System.Data.SQLite";

Console.WriteLine("Connection String: " + settings.ConnectionString);
Console.WriteLine("Provider Name: " + settings.ProviderInvariantName);

var project = new Project(settings);
project.Save(OutDir + "SupportForSQLiteDatabase_out.mpp", SaveFileFormat.Mpp);
```

### 另见

* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


