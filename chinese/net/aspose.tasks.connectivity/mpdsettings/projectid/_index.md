---
title: "MpdSettings.ProjectId"
second_title: "Aspose.Tasks for .NET API 参考"
description: "MpdSettings 属性。获取要读取的项目 ID"
type: docs
weight: 20
url: /zh/net/aspose.tasks.connectivity/mpdsettings/projectid/
---
## MpdSettings.ProjectId property

获取要读取的项目的 id。

```csharp
public int ProjectId { get; }
```

## 示例

展示如何使用 MPD 设置来控制从数据库导入项目。

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### 另见

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


