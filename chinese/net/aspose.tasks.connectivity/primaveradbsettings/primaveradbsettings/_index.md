---
title: "PrimaveraDbSettings.PrimaveraDbSettings"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PrimaveraDbSettings 构造函数。初始化 PrimaveraDbSettings 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks.connectivity/primaveradbsettings/primaveradbsettings/
---
## PrimaveraDbSettings constructor

初始化 [`PrimaveraDbSettings`](../) 类的新实例。

```csharp
public PrimaveraDbSettings(string connectionString, int projectId)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| connectionString | 字符串 | 指定的连接字符串。 |
| projectId | Int32 | 指定的要读取的项目 ID。 |

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

* class [PrimaveraDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../primaveradbsettings/)
* assembly [Aspose.Tasks](../../../)


