---
title: Class PrimaveraXmlReader
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.PrimaveraXmlReader class. Represents a reader which allows to retrieve Project UIDs from Primavera Xml file
type: docs
weight: 1390
url: /net/aspose.tasks/primaveraxmlreader/
---
## PrimaveraXmlReader class

Represents a reader which allows to retrieve Project UIDs from Primavera Xml file.

```csharp
public class PrimaveraXmlReader : PrimaveraBaseReader
```

## Constructors

| Name | Description |
| --- | --- |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor)(Stream) | Initializes a new instance of the `PrimaveraXmlReader` class. |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor_1)(string) | Initializes a new instance of the `PrimaveraXmlReader` class. |

## Methods

| Name | Description |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Return a list of the project's short info objects. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Return a list of the projects' unique identifiers. |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | Loads the project with the specified unique identifier. |

## Examples

Shows how to examine short projects' info from a Primavera XML file.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "MultiprojectWithExternal.xml");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}
```

### See Also

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


