---
title: "MpdSettings.MpdSettings"
second_title: "Aspose.Tasks for .NET API 参考"
description: "MpdSettings 构造函数。初始化 MpdSettings 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks.connectivity/mpdsettings/mpdsettings/
---
## MpdSettings constructor

初始化 [`MpdSettings`](../) 类的新实例。

```csharp
public MpdSettings(string connectionString, int projectId)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| connectionString | 字符串 | 指定的连接字符串。 |
| projectId | Int32 | 指定的要读取的项目 ID。 |

## 示例

展示如何从 MPD 文件读取项目。

```csharp
DbSettings settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### 另见

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


