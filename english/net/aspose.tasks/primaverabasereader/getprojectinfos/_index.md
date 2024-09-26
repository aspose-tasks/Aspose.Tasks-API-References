---
title: PrimaveraBaseReader.GetProjectInfos
second_title: Aspose.Tasks for .NET API Reference
description: PrimaveraBaseReader method. Return a list of the projects short info objects
type: docs
weight: 10
url: /net/aspose.tasks/primaverabasereader/getprojectinfos/
---
## PrimaveraBaseReader.GetProjectInfos method

Return a list of the project's short info objects.

```csharp
public List<PrimaveraProjectInfo> GetProjectInfos()
```

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

* class [PrimaveraProjectInfo](../../../aspose.tasks.primavera/primaveraprojectinfo/)
* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


