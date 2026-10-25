---
title: "DbSettings.ProviderInvariantName"
second_title: "Aspose.Tasks for .NET API 参考"
description: "DbSettings 属性。获取或设置提供程序不变名称，该名称用于获取 DbProviderFactory 类的实例。默认值为 SqlClient"
type: docs
weight: 40
url: /zh/net/aspose.tasks.connectivity/dbsettings/providerinvariantname/
---
## DbSettings.ProviderInvariantName property

获取或设置用于获取 DbProviderFactory 类实例的提供程序不变名称。默认值为 SqlClient。

```csharp
public string ProviderInvariantName { get; set; }
```

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

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


