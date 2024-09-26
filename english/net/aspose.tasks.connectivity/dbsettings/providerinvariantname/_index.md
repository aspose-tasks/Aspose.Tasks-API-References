---
title: DbSettings.ProviderInvariantName
second_title: Aspose.Tasks for .NET API Reference
description: DbSettings property. Gets or sets provider invariant name which is used to get an instance of the DbProviderFactory class. Default value is SqlClient
type: docs
weight: 20
url: /net/aspose.tasks.connectivity/dbsettings/providerinvariantname/
---
## DbSettings.ProviderInvariantName property

Gets or sets provider invariant name which is used to get an instance of the DbProviderFactory class. Default value is SqlClient.

```csharp
public string ProviderInvariantName { get; set; }
```

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

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


