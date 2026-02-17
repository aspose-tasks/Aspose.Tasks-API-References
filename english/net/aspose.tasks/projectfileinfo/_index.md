---
title: Class ProjectFileInfo
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ProjectFileInfo class. The class instance contains information about project file format and version of Microsoft Project where the file was created
type: docs
weight: 1440
url: /net/aspose.tasks/projectfileinfo/
---
## ProjectFileInfo class

The class instance contains information about project file format and version of Microsoft Project where the file was created.

```csharp
public sealed class ProjectFileInfo : IEquatable<ProjectFileInfo>
```

## Properties

| Name | Description |
| --- | --- |
| [CanRead](../../aspose.tasks/projectfileinfo/canread/) { get; } | Gets a value indicating whether defines can Aspose.Tasks process the project file. |
| [IsPasswordProtected](../../aspose.tasks/projectfileinfo/ispasswordprotected/) { get; } | Gets a value indicating whether a project is password protected. |
| [ProjectApplicationInfo](../../aspose.tasks/projectfileinfo/projectapplicationinfo/) { get; } | Gets project file application info. |
| [ProjectFileFormat](../../aspose.tasks/projectfileinfo/projectfileformat/) { get; } | Gets project file format. |

## Methods

| Name | Description |
| --- | --- |
| override [Equals](../../aspose.tasks/projectfileinfo/equals/#equals_1)(object) | Returns a value indicating whether this instance is equal to a specified object. |
| [Equals](../../aspose.tasks/projectfileinfo/equals/#equals)(ProjectFileInfo) | Returns a value indicating whether this instance is equal to a specified object. |
| override [GetHashCode](../../aspose.tasks/projectfileinfo/gethashcode/)() | Returns a hash code value for the instance of the `ProjectFileInfo` class. |

## Remarks

Use CanRead property to define that the library can process the project file.

## Examples

Shows how to read project file info.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


