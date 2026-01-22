---
title: PrimaveraDbSettings.ProjectId
second_title: Aspose.Tasks for .NET API Reference
description: PrimaveraDbSettings property. Gets id of the project to read
type: docs
weight: 20
url: /net/aspose.tasks.connectivity/primaveradbsettings/projectid/
---
## PrimaveraDbSettings.ProjectId property

Gets id of the project to read.

```csharp
public int ProjectId { get; }
```

## Examples

Shows how to import a project from a Primavera database.

```csharp
// Initialize a new instance of the PrimaveraDbSettings class with connection string and project id
var settings = new PrimaveraDbSettings(GetConnectionString(), 4502);

Console.WriteLine("Project UID to read: " + settings.ProjectId);

// read the project with UID = 4502
var project = new Project(settings);
Console.WriteLine(project.Uid);
Console.WriteLine(project.Name);
Console.WriteLine(project.PrimaveraProperties.ShortName);
```

### See Also

* class [PrimaveraDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../primaveradbsettings/)
* assembly [Aspose.Tasks](../../../)


