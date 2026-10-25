---
title: "Classe MspDbSettings"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Connectivity.MspDbSettings. Consente di impostare le opzioni necessarie per leggere i dati del progetto dal database di MS Project Server"
type: docs
weight: 310
url: /it/net/aspose.tasks.connectivity/mspdbsettings/
---
## MspDbSettings class

Consente di impostare le opzioni necessarie per leggere i dati del progetto dal database MS Project Server.

```csharp
public class MspDbSettings : DbSettings
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [MspDbSettings](mspdbsettings/)(string, Guid) | Inizializza una nuova istanza della classe `MspDbSettings`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Ottiene o imposta la stringa di connessione. |
| [ProjectGuid](../../aspose.tasks.connectivity/mspdbsettings/projectguid/) { get; } | Ottiene il guid del progetto da leggere. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Ottiene o imposta la callback da invocare durante le operazioni di caricamento del progetto. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Ottiene o imposta un'istanza di DbProviderFactory utilizzata per connettersi al DB. Se sia ProviderFactory sia ProviderInvariantName sono impostati, ProviderFactory ha la priorità. Il valore predefinito è null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Ottiene o imposta il nome invariabile del provider utilizzato per ottenere un'istanza della classe DbProviderFactory. Il valore predefinito è SqlClient. |
| [Schema](../../aspose.tasks.connectivity/mspdbsettings/schema/) { get; set; } | Ottiene o imposta lo schema di MS Project Server. Il valore predefinito è \"pub\". |

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

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


