---
title: DbSettings.ProviderFactory
second_title: Aspose.Tasks for .NET API Reference
description: DbSettings property. Gets or sets an instance of DbProviderFactory which is used to connect to DB. If both ProviderFactory and ProviderInvariantName are set ProviderFactory has a priority. Default value is null
type: docs
weight: 30
url: /net/aspose.tasks.connectivity/dbsettings/providerfactory/
---
## DbSettings.ProviderFactory property

Gets or sets an instance of DbProviderFactory which is used to connect to DB. If both ProviderFactory and ProviderInvariantName are set, ProviderFactory has a priority. Default value is null.

```csharp
public DbProviderFactory ProviderFactory { get; set; }
```

## Examples

Shows how to import a project from a Primavera database.

```csharp
// Initialize a new instance of the PrimaveraDbSettings class with connection string and project id
var settings = new PrimaveraDbSettings(GetConnectionString(), 4502);
settings.ProviderFactory = SqliteFactory.Instance;

Console.WriteLine("Project UID to read: " + settings.ProjectId);

// read the project with UID = 4502
var project = new Project(settings);
Console.WriteLine(project.Uid);
Console.WriteLine(project.Name);
Console.WriteLine(project.PrimaveraProperties.ShortName);
```

### See Also

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


