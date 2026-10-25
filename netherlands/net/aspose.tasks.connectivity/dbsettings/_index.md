---
title: "Klasse DbSettings"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Connectivity.DbSettings class. Stelt u in staat om instellingen op te geven om te lezen uit een projectdatabase"
type: docs
weight: 290
url: /nl/net/aspose.tasks.connectivity/dbsettings/
---
## DbSettings class

Staat toe instellingen te specificeren om uit de projectdatabase te lezen.

```csharp
public abstract class DbSettings
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Haalt op of stelt de verbindingsreeks in. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Haalt op of stelt de callback in die wordt aangeroepen tijdens projectlaadbewerkingen. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Haalt op of stelt een instantie van DbProviderFactory in die wordt gebruikt om verbinding te maken met de database. Als zowel ProviderFactory als ProviderInvariantName zijn ingesteld, heeft ProviderFactory prioriteit. Standaardwaarde is null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Haalt op of stelt de provider-invariante naam in die wordt gebruikt om een instantie van de DbProviderFactory klasse te verkrijgen. Standaardwaarde is SqlClient. |

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

* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


