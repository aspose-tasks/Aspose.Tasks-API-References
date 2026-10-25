---
title: "DbSettings.ConnectionString"
second_title: "Aspose.Tasks for .NET API 参考"
description: "DbSettings 属性。获取或设置连接字符串"
type: docs
weight: 10
url: /zh/net/aspose.tasks.connectivity/dbsettings/connectionstring/
---
## DbSettings.ConnectionString property

获取或设置连接字符串。

```csharp
public string ConnectionString { get; set; }
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


