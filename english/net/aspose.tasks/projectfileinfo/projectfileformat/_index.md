---
title: ProjectFileInfo.ProjectFileFormat
second_title: Aspose.Tasks for .NET API Reference
description: ProjectFileInfo property. Gets project file format
type: docs
weight: 40
url: /net/aspose.tasks/projectfileinfo/projectfileformat/
---
## ProjectFileInfo.ProjectFileFormat property

Gets project file format.

```csharp
public FileFormat ProjectFileFormat { get; }
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

* enum [FileFormat](../../fileformat/)
* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


