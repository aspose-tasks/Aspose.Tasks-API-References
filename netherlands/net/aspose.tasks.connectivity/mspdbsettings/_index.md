---
title: "Klasse MspDbSettings"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Connectivity.MspDbSettings class. Stelt u in staat om de benodigde opties in te stellen om projectgegevens te lezen uit een MS Project Server-database"
type: docs
weight: 310
url: /nl/net/aspose.tasks.connectivity/mspdbsettings/
---
## MspDbSettings class

Staat toe om de benodigde opties in te stellen om projectgegevens te lezen uit de MS Project Server‑database.

```csharp
public class MspDbSettings : DbSettings
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [MspDbSettings](mspdbsettings/)(string, Guid) | Initialiseert een nieuw exemplaar van de `MspDbSettings` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Haalt op of stelt de verbindingsreeks in. |
| [ProjectGuid](../../aspose.tasks.connectivity/mspdbsettings/projectguid/) { get; } | Haalt de GUID van het te lezen project op. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Haalt op of stelt de callback in die wordt aangeroepen tijdens projectlaadbewerkingen. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Haalt op of stelt een instantie van DbProviderFactory in die wordt gebruikt om verbinding te maken met de database. Als zowel ProviderFactory als ProviderInvariantName zijn ingesteld, heeft ProviderFactory prioriteit. Standaardwaarde is null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Haalt op of stelt de provider-invariante naam in die wordt gebruikt om een instantie van de DbProviderFactory klasse te verkrijgen. Standaardwaarde is SqlClient. |
| [Schema](../../aspose.tasks.connectivity/mspdbsettings/schema/) { get; set; } | Haalt op of stelt het schema van de MS Project Server in. De standaardwaarde is "pub". |

## Voorbeelden

Toont hoe een project uit een database te importeren.

```csharp
try
{
    // Maak verbindingsreeks
    var connectionString = new SqlConnectionStringBuilder();
    connectionString.DataSource = "192.168.56.2,1433";
    connectionString.Encrypt = true;
    connectionString.TrustServerCertificate = true;
    connectionString.InitialCatalog = "ProjectServer_Published";
    connectionString.NetworkLibrary = "DBMSSOCN";
    connectionString.UserID = "sa";
    connectionString.Password = "*****";

    // maak instellingen om te laden vanuit MS-database
    var settings = new MspDbSettings(connectionString.ConnectionString, new Guid("E6426C44-D6CB-4B9C-AF16-48910ACE0F54"));
    settings.Schema = "dbo";

    Console.WriteLine("Project GUID to load: " + settings.ProjectGuid);

    var project = new Project(settings);

    project.Save(OutDir + "ImportProjectDataFromDatabase_out.mpp", SaveFileFormat.Mpp);
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message + " Please setup proper data source (DataSource, InitialCatalog etc)");
}
```

### Zie ook

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


