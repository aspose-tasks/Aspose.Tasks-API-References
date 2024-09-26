---
title: PrimaveraBaseReader.GetProjectUids
second_title: Aspose.Tasks for .NET API Reference
description: PrimaveraBaseReader method. Return a list of the projects unique identifiers
type: docs
weight: 20
url: /net/aspose.tasks/primaverabasereader/getprojectuids/
---
## PrimaveraBaseReader.GetProjectUids method

Return a list of the projects' unique identifiers.

```csharp
public List<int> GetProjectUids()
```

### Return Value

List of projects' unique identifiers.

## Examples

Shows how to import a project from a Primavera XML file.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "primavera.xml");
List<int> projectUids = reader.GetProjectUids();
foreach (var projectUid in projectUids)
{
    Console.WriteLine("Project UID: " + projectUid);
}
```

### See Also

* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


