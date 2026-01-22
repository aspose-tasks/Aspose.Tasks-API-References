---
title: Class PrimaveraDbSettings
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Connectivity.PrimaveraDbSettings class. Allows to set necessary options to read project data from Primavera database
type: docs
weight: 320
url: /net/aspose.tasks.connectivity/primaveradbsettings/
---
## PrimaveraDbSettings class

Allows to set necessary options to read project data from Primavera database.

```csharp
public class PrimaveraDbSettings : DbSettings
```

## Constructors

| Name | Description |
| --- | --- |
| [PrimaveraDbSettings](primaveradbsettings/)(string, int) | Initializes a new instance of the `PrimaveraDbSettings` class. |

## Properties

| Name | Description |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Gets or sets the connection string. |
| [ProjectId](../../aspose.tasks.connectivity/primaveradbsettings/projectid/) { get; } | Gets id of the project to read. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Gets or sets provider invariant name which is used to get an instance of the DbProviderFactory class. Default value is SqlClient. |

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

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


