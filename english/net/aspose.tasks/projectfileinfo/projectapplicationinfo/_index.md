---
title: ProjectFileInfo.ProjectApplicationInfo
second_title: Aspose.Tasks for .NET API Reference
description: ProjectFileInfo property. Gets project file application info
type: docs
weight: 30
url: /net/aspose.tasks/projectfileinfo/projectapplicationinfo/
---
## ProjectFileInfo.ProjectApplicationInfo property

Gets project file application info.

```csharp
public ApplicationInfo ProjectApplicationInfo { get; }
```

## Examples

Shows how to read project file info.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### See Also

* enum [ApplicationInfo](../../applicationinfo/)
* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


