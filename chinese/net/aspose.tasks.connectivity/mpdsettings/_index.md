---
title: "类 MpdSettings"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Connectivity.MpdSettings 类。允许设置读取 MPD 格式 MS Access 数据库文件格式的项目数据所需的选项"
type: docs
weight: 300
url: /zh/net/aspose.tasks.connectivity/mpdsettings/
---
## MpdSettings class

允许设置必要的选项以从 MPD 格式（MS Access 数据库文件格式）读取项目数据。

```csharp
public class MpdSettings : DbSettings
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [MpdSettings](mpdsettings/)(string, int) | 初始化 `MpdSettings` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | 获取或设置连接字符串。 |
| [ProjectId](../../aspose.tasks.connectivity/mpdsettings/projectid/) { get; } | 获取要读取的项目的 id。 |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | 获取或设置在项目加载操作期间调用的回调函数。 |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | 获取或设置用于连接数据库的 DbProviderFactory 实例。如果同时设置了 ProviderFactory 和 ProviderInvariantName，则 ProviderFactory 优先。默认值为 null。 |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | 获取或设置用于获取 DbProviderFactory 类实例的提供程序不变名称。默认值为 SqlClient。 |

## 示例

展示如何使用 MPD 设置来控制从数据库导入项目。

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### 另见

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


