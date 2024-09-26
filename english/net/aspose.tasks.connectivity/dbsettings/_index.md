---
title: Class DbSettings
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Connectivity.DbSettings class. Allows to specify settings to read from project database
type: docs
weight: 290
url: /net/aspose.tasks.connectivity/dbsettings/
---
## DbSettings class

Allows to specify settings to read from project database.

```csharp
public abstract class DbSettings
```

## Properties

| Name | Description |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Gets or sets the connection string. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Gets or sets provider invariant name which is used to get an instance of the DbProviderFactory class. Default value is SqlClient. |

## Examples

Shows how to read a project from a Primavera XML file with multiple projects by using a provider name.

```csharp
var connectionString = "Data Source=" + DataDir + "\\PPMDBSQLite.db";

// Create Primavera DB Settings using connection string and project id
var settings = new PrimaveraDbSettings(connectionString, 4502);
settings.ProviderInvariantName = "System.Data.SQLite";

Console.WriteLine("Connection String: " + settings.ConnectionString);
Console.WriteLine("Provider Name: " + settings.ProviderInvariantName);

var project = new Project(settings);
project.Save(OutDir + "SupportForSQLiteDatabase_out.mpp", SaveFileFormat.Mpp);
```

### See Also

* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


