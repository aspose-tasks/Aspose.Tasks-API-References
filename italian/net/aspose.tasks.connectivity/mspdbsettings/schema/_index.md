---
title: "MspDbSettings.Schema"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà MspDbSettings. Ottiene o imposta lo schema del MS Project Server. Il valore predefinito è pub"
type: docs
weight: 30
url: /it/net/aspose.tasks.connectivity/mspdbsettings/schema/
---
## MspDbSettings.Schema property

Ottiene o imposta lo schema di MS Project Server. Il valore predefinito è \"pub\".

```csharp
public string Schema { get; set; }
```

## Esempi

Mostra come importare un progetto da un database.

```csharp
try
{
    // Crea la stringa di connessione
    var connectionString = new SqlConnectionStringBuilder();
    connectionString.DataSource = "192.168.56.2,1433";
    connectionString.Encrypt = true;
    connectionString.TrustServerCertificate = true;
    connectionString.InitialCatalog = "ProjectServer_Published";
    connectionString.NetworkLibrary = "DBMSSOCN";
    connectionString.UserID = "sa";
    connectionString.Password = "*****";

    // crea impostazioni per caricare dal database MS
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

### Vedi anche

* class [MspDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mspdbsettings/)
* assembly [Aspose.Tasks](../../../)


