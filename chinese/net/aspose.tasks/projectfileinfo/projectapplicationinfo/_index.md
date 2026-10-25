---
title: "ProjectFileInfo.ProjectApplicationInfo"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProjectFileInfo 属性。获取项目文件的应用信息"
type: docs
weight: 30
url: /zh/net/aspose.tasks/projectfileinfo/projectapplicationinfo/
---
## ProjectFileInfo.ProjectApplicationInfo property

获取项目文件的应用程序信息。

```csharp
public ApplicationInfo ProjectApplicationInfo { get; }
```

## 示例

展示如何读取项目文件信息。

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### 另见

* enum [ApplicationInfo](../../applicationinfo/)
* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


