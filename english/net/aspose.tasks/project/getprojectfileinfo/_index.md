---
title: Project.GetProjectFileInfo
second_title: Aspose.Tasks for .NET API Reference
description: Project method. Read project file info from the file
type: docs
weight: 1290
url: /net/aspose.tasks/project/getprojectfileinfo/
---
## GetProjectFileInfo(string) {#getprojectfileinfo_1}

Read project file info from the file.

```csharp
public static ProjectFileInfo GetProjectFileInfo(string filename)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filename | String | The project filename. |

### Return Value

The project file info [`ProjectFileInfo`](../../projectfileinfo/).

## Examples

Shows how to read project file info were read from an XML file.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### See Also

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetProjectFileInfo(Stream) {#getprojectfileinfo}

Gets project file info from the stream.

```csharp
public static ProjectFileInfo GetProjectFileInfo(Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The data stream. |

### Return Value

The project file info [`ProjectFileInfo`](../../projectfileinfo/).

## Examples

Shows how to read project file info of XML file read from a stream.

```csharp
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var info = Project.GetProjectFileInfo(stream);
    Console.WriteLine("CanRead: " + info.CanRead);
    Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
    Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
}
```

### See Also

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


