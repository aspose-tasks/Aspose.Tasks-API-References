---
title: ProjectFileInfo.GetHashCode
second_title: Aspose.Tasks for .NET API Reference
description: ProjectFileInfo method. Returns a hash code value for the instance of the ProjectFileInfo class
type: docs
weight: 60
url: /net/aspose.tasks/projectfileinfo/gethashcode/
---
## ProjectFileInfo.GetHashCode method

Returns a hash code value for the instance of the [`ProjectFileInfo`](../) class.

```csharp
public override int GetHashCode()
```

### Return Value

returns a hash code value for this object.

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


