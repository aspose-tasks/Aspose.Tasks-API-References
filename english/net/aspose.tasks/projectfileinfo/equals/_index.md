---
title: ProjectFileInfo.Equals
second_title: Aspose.Tasks for .NET API Reference
description: ProjectFileInfo method. Returns a value indicating whether this instance is equal to a specified object
type: docs
weight: 50
url: /net/aspose.tasks/projectfileinfo/equals/
---
## Equals(ProjectFileInfo) {#equals}

Returns a value indicating whether this instance is equal to a specified object.

```csharp
public bool Equals(ProjectFileInfo other)
```

| Parameter | Type | Description |
| --- | --- | --- |
| other | ProjectFileInfo | The specified object to compare with this instance. |

### Return Value

returns true if the specified ProjectFileInfo and this instance have equal file format and application info.

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

---

## Equals(object) {#equals_1}

Returns a value indicating whether this instance is equal to a specified object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The specified object to compare with this instance. |

### Return Value

returns true if the specified ProjectFileInfo and this instance have equal file format and application info.

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


