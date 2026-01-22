---
title: Class PrimaveraDbReader
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.PrimaveraDbReader class. Represents a reader to read Project Info from Primavera DB
type: docs
weight: 1330
url: /net/aspose.tasks/primaveradbreader/
---
## PrimaveraDbReader class

Represents a reader to read Project Info from Primavera DB

```csharp
public sealed class PrimaveraDbReader : PrimaveraBaseReader
```

## Constructors

| Name | Description |
| --- | --- |
| [PrimaveraDbReader](primaveradbreader/)(PrimaveraDbSettings) | Initializes a new instance of the [`PrimaveraXerReader`](../primaveraxerreader/) class. |

## Methods

| Name | Description |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Return a list of the project's short info objects. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Return a list of the projects' unique identifiers. |
| override [LoadProject](../../aspose.tasks/primaveradbreader/loadproject/)(int) | Loads the project with the specified unique identifier. |

## Examples

Shows how to get brief info of projects from a Primavera database.

```csharp
var settings = new PrimaveraDbSettings(GetConnectionString(), 0);

var reader = new PrimaveraDbReader(settings);
var projectInfos = reader.GetProjectInfos();

foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - '{2}'", info.Uid, info.ShortName, info.Name);
}

var firstProject = reader.LoadProject(projectInfos[0].Uid);
Console.WriteLine(firstProject.Uid);
Console.WriteLine(firstProject.Name);
Console.WriteLine(firstProject.PrimaveraProperties.ShortName);
```

### See Also

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


