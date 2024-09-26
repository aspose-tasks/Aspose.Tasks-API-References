---
title: Class MpdSettings
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Connectivity.MpdSettings class. Allows to set necessary options to read project data from MPD format MS Access database file format
type: docs
weight: 300
url: /net/aspose.tasks.connectivity/mpdsettings/
---
## MpdSettings class

Allows to set necessary options to read project data from MPD format (MS Access database file format).

```csharp
public class MpdSettings : DbSettings
```

## Constructors

| Name | Description |
| --- | --- |
| [MpdSettings](mpdsettings/)(string, int) | Initializes a new instance of the `MpdSettings` class. |

## Properties

| Name | Description |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Gets or sets the connection string. |
| [ProjectId](../../aspose.tasks.connectivity/mpdsettings/projectid/) { get; } | Gets id of the project to read. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Gets or sets provider invariant name which is used to get an instance of the DbProviderFactory class. Default value is SqlClient. |

## Examples

Shows how to use MPD settings to control import of project from the database.

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### See Also

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


