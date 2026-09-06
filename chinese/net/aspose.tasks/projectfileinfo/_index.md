---
title: "类 ProjectFileInfo"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.ProjectFileInfo 类。该类实例包含有关项目文件格式以及创建文件时使用的 Microsoft Project 版本的信息。"
type: docs
weight: 1460
url: /zh/net/aspose.tasks/projectfileinfo/
---
## ProjectFileInfo class

该类实例包含有关项目文件格式以及创建该文件的 Microsoft Project 版本的信息。

```csharp
public sealed class ProjectFileInfo : IEquatable<ProjectFileInfo>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [CanRead](../../aspose.tasks/projectfileinfo/canread/) { get; } | 获取一个值，指示 Aspose.Tasks 是否可以处理该项目文件。 |
| [IsPasswordProtected](../../aspose.tasks/projectfileinfo/ispasswordprotected/) { get; } | 获取一个值，指示项目是否受密码保护。 |
| [ProjectApplicationInfo](../../aspose.tasks/projectfileinfo/projectapplicationinfo/) { get; } | 获取项目文件的应用程序信息。 |
| [ProjectFileFormat](../../aspose.tasks/projectfileinfo/projectfileformat/) { get; } | 获取项目文件格式。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [Equals](../../aspose.tasks/projectfileinfo/equals/#equals_1)(object) | 返回一个值，指示此实例是否等于指定的对象。 |
| [Equals](../../aspose.tasks/projectfileinfo/equals/#equals)(ProjectFileInfo) | 返回一个值，指示此实例是否等于指定的对象。 |
| override [GetHashCode](../../aspose.tasks/projectfileinfo/gethashcode/)() | 返回 `ProjectFileInfo` 类实例的哈希码值。 |

## 备注

使用 CanRead 属性来定义库可以处理项目文件。

## 示例

展示如何读取项目文件信息。

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


