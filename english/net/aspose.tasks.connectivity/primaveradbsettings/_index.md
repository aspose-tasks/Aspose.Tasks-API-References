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
var sb = new SqlConnectionStringBuilder();
sb.DataSource = "192.168.56.3,1433";
sb.Encrypt = true;
sb.TrustServerCertificate = true;
sb.InitialCatalog = "PrimaveraEDB";
sb.NetworkLibrary = "DBMSSOCN";
sb.UserID = "privuser";
sb.Password = "***";

// Initialize a new instance of the PrimaveraDbSettings class with connection string and project id
var settings = new PrimaveraDbSettings(sb.ConnectionString, 4502);

Console.WriteLine("Project UID to read: " + settings.ProjectId);

// read the project with UID = 4502
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Uid));
```

### See Also

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


