---
title: PrimaveraBaseReader.LoadProject
second_title: Aspose.Tasks for .NET API Reference
description: PrimaveraBaseReader method. Loads the project with the specified unique identifier
type: docs
weight: 30
url: /net/aspose.tasks/primaverabasereader/loadproject/
---
## PrimaveraBaseReader.LoadProject method

Loads the project with the specified unique identifier.

```csharp
public virtual Project LoadProject(int projectUid)
```

| Parameter | Type | Description |
| --- | --- | --- |
| projectUid | Int32 | Unique identifier of the project to load. |

### Return Value

Project with specified unique identifier from the specified multi project file. Null if project doesn't exist.

## Examples

Shows how to load a project from a Primavera XML file when project uid is known.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "PrimaveraProject.xml");
var project = reader.LoadProject(3882);
Console.WriteLine(project.Name);
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

* class [Project](../../project/)
* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


