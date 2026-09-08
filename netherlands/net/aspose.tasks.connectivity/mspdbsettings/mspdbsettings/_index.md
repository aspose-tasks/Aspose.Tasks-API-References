---
title: "MspDbSettings.MspDbSettings"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "MspDbSettings constructor. Initialiseert een nieuw exemplaar van de MspDbSettings-klasse"
type: docs
weight: 10
url: /nl/net/aspose.tasks.connectivity/mspdbsettings/mspdbsettings/
---
## MspDbSettings constructor

Initialiseert een nieuw exemplaar van de [`MspDbSettings`](../) klasse.

```csharp
public MspDbSettings(string connectionString, Guid projectGuid)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| connectionString | String | de opgegeven connection string. |
| projectGuid | Guid | de opgegeven guid van een project om te lezen. |

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

* class [MspDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mspdbsettings/)
* assembly [Aspose.Tasks](../../../)


