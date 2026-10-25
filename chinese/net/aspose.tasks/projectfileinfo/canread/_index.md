---
title: "ProjectFileInfo.CanRead"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProjectFileInfo 属性。获取一个值，指示是否可以让 Aspose.Tasks 处理项目文件"
type: docs
weight: 10
url: /zh/net/aspose.tasks/projectfileinfo/canread/
---
## ProjectFileInfo.CanRead property

获取一个值，指示 Aspose.Tasks 是否可以处理该项目文件。

```csharp
public bool CanRead { get; }
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

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


