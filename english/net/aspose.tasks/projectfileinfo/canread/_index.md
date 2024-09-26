---
title: ProjectFileInfo.CanRead
second_title: Aspose.Tasks for .NET API Reference
description: ProjectFileInfo property. Gets a value indicating whether defines can Aspose.Tasks process the project file
type: docs
weight: 10
url: /net/aspose.tasks/projectfileinfo/canread/
---
## ProjectFileInfo.CanRead property

Gets a value indicating whether defines can Aspose.Tasks process the project file.

```csharp
public bool CanRead { get; }
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

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


