---
title: "DbSettings.ProviderFactory"
second_title: "Aspose.Tasks for .NET API 参考"
description: "DbSettings 属性。获取或设置用于连接数据库的 DbProviderFactory 实例。如果同时设置了 ProviderFactory 和 ProviderInvariantName，则 ProviderFactory 优先。默认值为 null"
type: docs
weight: 30
url: /zh/net/aspose.tasks.connectivity/dbsettings/providerfactory/
---
## DbSettings.ProviderFactory property

获取或设置用于连接数据库的 DbProviderFactory 实例。如果同时设置了 ProviderFactory 和 ProviderInvariantName，则 ProviderFactory 优先。默认值为 null。

```csharp
public DbProviderFactory ProviderFactory { get; set; }
```

## 示例

展示如何从 Primavera 数据库导入项目。

```csharp
// 使用连接字符串和项目 id 初始化 PrimaveraDbSettings 类的新实例
var settings = new PrimaveraDbSettings(GetConnectionString(), 4502);
settings.ProviderFactory = SqliteFactory.Instance;

Console.WriteLine("Project UID to read: " + settings.ProjectId);

// 读取 UID = 4502 的项目
var project = new Project(settings);
Console.WriteLine(project.Uid);
Console.WriteLine(project.Name);
Console.WriteLine(project.PrimaveraProperties.ShortName);
```

### 另见

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


