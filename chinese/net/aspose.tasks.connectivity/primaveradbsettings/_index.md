---
title: "类 PrimaveraDbSettings"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Connectivity.PrimaveraDbSettings 类。允许设置读取 Primavera 数据库的项目数据所需的选项"
type: docs
weight: 320
url: /zh/net/aspose.tasks.connectivity/primaveradbsettings/
---
## PrimaveraDbSettings class

允许设置必要的选项以从 Primavera 数据库读取项目数据。

```csharp
public class PrimaveraDbSettings : DbSettings
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [PrimaveraDbSettings](primaveradbsettings/)(string, int) | 初始化 `PrimaveraDbSettings` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | 获取或设置连接字符串。 |
| [ProjectId](../../aspose.tasks.connectivity/primaveradbsettings/projectid/) { get; } | 获取要读取的项目的 id。 |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | 获取或设置在项目加载操作期间调用的回调函数。 |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | 获取或设置用于连接数据库的 DbProviderFactory 实例。如果同时设置了 ProviderFactory 和 ProviderInvariantName，则 ProviderFactory 优先。默认值为 null。 |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | 获取或设置用于获取 DbProviderFactory 类实例的提供程序不变名称。默认值为 SqlClient。 |

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

展示如何从 Primavera 数据库获取项目的简要信息。

```csharp
var settings = new PrimaveraDbSettings(GetConnectionString(), 0);

var reader = new PrimaveraDbReader(settings);
var projectInfos = reader.GetProjectInfos();

foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - '{2}'", info.Uid, info.ShortName, info.Name);
}

var firstProject = reader.LoadProject(projectInfos[0].Uid);
Console.WriteLine(firstProject.Uid);
Console.WriteLine(firstProject.Name);
Console.WriteLine(firstProject.PrimaveraProperties.ShortName);
```

### 另见

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


