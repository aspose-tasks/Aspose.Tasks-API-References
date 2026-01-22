---
title: PrimaveraDbSettings.PrimaveraDbSettings
second_title: Aspose.Tasks for .NET API Reference
description: PrimaveraDbSettings constructor. Initializes a new instance of the PrimaveraDbSettings class
type: docs
weight: 10
url: /net/aspose.tasks.connectivity/primaveradbsettings/primaveradbsettings/
---
## PrimaveraDbSettings constructor

Initializes a new instance of the [`PrimaveraDbSettings`](../) class.

```csharp
public PrimaveraDbSettings(string connectionString, int projectId)
```

| Parameter | Type | Description |
| --- | --- | --- |
| connectionString | String | the specified connection string. |
| projectId | Int32 | the specified id of a project to read. |

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


