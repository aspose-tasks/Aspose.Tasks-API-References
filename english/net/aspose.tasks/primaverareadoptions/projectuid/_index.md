---
title: PrimaveraReadOptions.ProjectUid
second_title: Aspose.Tasks for .NET API Reference
description: PrimaveraReadOptions property. Gets or sets the UID of a project to read from file containing multiple projects
type: docs
weight: 30
url: /net/aspose.tasks/primaverareadoptions/projectuid/
---
## PrimaveraReadOptions.ProjectUid property

Gets or sets the UID of a project to read from file containing multiple projects.

```csharp
public int ProjectUid { get; set; }
```

## Examples

Shows how to read a project from a Primavera XML or Primavera XER file containing multiple projects.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 3881;

// Returns project with special Uid
var project = new Project(DataDir + "PrimaveraProject.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### See Also

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


