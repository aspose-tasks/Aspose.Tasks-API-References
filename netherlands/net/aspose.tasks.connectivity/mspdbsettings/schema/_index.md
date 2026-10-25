---
title: "MspDbSettings.Schema"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "MspDbSettings eigenschap. Haalt op of stelt het schema van de MS Project Server in. De standaardwaarde is pub"
type: docs
weight: 30
url: /nl/net/aspose.tasks.connectivity/mspdbsettings/schema/
---
## MspDbSettings.Schema property

Haalt op of stelt het schema van de MS Project Server in. De standaardwaarde is "pub".

```csharp
public string Schema { get; set; }
```

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


