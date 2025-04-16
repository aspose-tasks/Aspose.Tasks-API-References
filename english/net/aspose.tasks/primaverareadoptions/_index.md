---
title: Class PrimaveraReadOptions
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.PrimaveraReadOptions class. Allows to specify additional options when reading Primavera Xml or Primavera Xer files
type: docs
weight: 1320
url: /net/aspose.tasks/primaverareadoptions/
---
## PrimaveraReadOptions class

Allows to specify additional options when reading Primavera Xml or Primavera Xer files.

```csharp
public class PrimaveraReadOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [PrimaveraReadOptions](primaverareadoptions/)() | Initializes a new instance of the `PrimaveraReadOptions` class. |

## Properties

| Name | Description |
| --- | --- |
| [PreserveUids](../../aspose.tasks/primaverareadoptions/preserveuids/) { get; set; } | Gets or sets a flag that specifies whether original unique identifiers of entities should be preserved. |
| [ProjectUid](../../aspose.tasks/primaverareadoptions/projectuid/) { get; set; } | Gets or sets the UID of a project to read from file containing multiple projects. |
| [ReadBaselineProjects](../../aspose.tasks/primaverareadoptions/readbaselineprojects/) { get; set; } | Gets or sets a flag that specifies whether baseline projects should be loaded. The default value is true. |
| [UndefinedConstraintHandlingBehavior](../../aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/) { get; set; } | Specifies the behavior used to process tasks with undefined constraints read from XER format. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


