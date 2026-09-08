---
title: "DbSettings.ProviderInvariantName"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "DbSettings eigenschap. Haalt op of stelt provider invariant name in die wordt gebruikt om een instantie van de DbProviderFactory-klasse te verkrijgen. Standaardwaarde is SqlClient"
type: docs
weight: 40
url: /nl/net/aspose.tasks.connectivity/dbsettings/providerinvariantname/
---
## DbSettings.ProviderInvariantName property

Haalt op of stelt de provider-invariante naam in die wordt gebruikt om een instantie van de DbProviderFactory klasse te verkrijgen. Standaardwaarde is SqlClient.

```csharp
public string ProviderInvariantName { get; set; }
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


