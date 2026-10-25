---
title: "DbSettings.ConnectionString"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "DbSettings eigenschap. Haalt op of stelt de connection string in"
type: docs
weight: 10
url: /nl/net/aspose.tasks.connectivity/dbsettings/connectionstring/
---
## DbSettings.ConnectionString property

Haalt op of stelt de verbindingsreeks in.

```csharp
public string ConnectionString { get; set; }
```

## Voorbeelden

Toont hoe een project te lezen uit een Primavera XML-bestand met meerdere projecten door een providernaam te gebruiken.

```csharp
var connectionString = "Data Source=" + DataDir + "\\PPMDBSQLite.db";

// Maak Primavera DB-instellingen met behulp van verbindingsreeks en project-ID
var settings = new PrimaveraDbSettings(connectionString, 4502);
settings.ProviderInvariantName = "System.Data.SQLite";

Console.WriteLine("Connection String: " + settings.ConnectionString);
Console.WriteLine("Provider Name: " + settings.ProviderInvariantName);

var project = new Project(settings);
project.Save(OutDir + "SupportForSQLiteDatabase_out.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


