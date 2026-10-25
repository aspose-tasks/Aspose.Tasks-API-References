---
title: "ProjectFileInfo.ProjectFileFormat"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProjectFileInfo 属性。获取项目文件格式"
type: docs
weight: 40
url: /zh/net/aspose.tasks/projectfileinfo/projectfileformat/
---
## ProjectFileInfo.ProjectFileFormat property

获取项目文件格式。

```csharp
public FileFormat ProjectFileFormat { get; }
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

* enum [FileFormat](../../fileformat/)
* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


