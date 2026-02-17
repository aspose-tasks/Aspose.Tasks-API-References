---
title: Class PrimaveraXerReader
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.PrimaveraXerReader class. Represents a reader to read Project UIDs from Primavera XER file
type: docs
weight: 1380
url: /net/aspose.tasks/primaveraxerreader/
---
## PrimaveraXerReader class

Represents a reader to read Project UIDs from Primavera XER file

```csharp
public sealed class PrimaveraXerReader : PrimaveraBaseReader
```

## Constructors

| Name | Description |
| --- | --- |
| [PrimaveraXerReader](primaveraxerreader/#constructor)(Stream) | Initializes a new instance of the `PrimaveraXerReader` class. |
| [PrimaveraXerReader](primaveraxerreader/#constructor_1)(string) | Initializes a new instance of the `PrimaveraXerReader` class. |

## Methods

| Name | Description |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Return a list of the project's short info objects. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Return a list of the projects' unique identifiers. |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | Loads the project with the specified unique identifier. |

## Examples

Shows how to examine short projects' info from a Primavera XER file.

```csharp
var reader = new PrimaveraXerReader(DataDir + "MultiprojectWithExternal.xer");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}

var project = reader.LoadProject(5494);

Console.WriteLine("Loaded project '{0}' with Uid {1}", project.Name, project.Uid);
```

### See Also

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


