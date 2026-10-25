---
title: "Classe DbSettings"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Connectivity.DbSettings. Consente di specificare le impostazioni per leggere dal database del progetto"
type: docs
weight: 290
url: /it/net/aspose.tasks.connectivity/dbsettings/
---
## DbSettings class

Consente di specificare le impostazioni per leggere dal database del progetto.

```csharp
public abstract class DbSettings
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Ottiene o imposta la stringa di connessione. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Ottiene o imposta la callback da invocare durante le operazioni di caricamento del progetto. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Ottiene o imposta un'istanza di DbProviderFactory utilizzata per connettersi al DB. Se sia ProviderFactory sia ProviderInvariantName sono impostati, ProviderFactory ha la priorità. Il valore predefinito è null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Ottiene o imposta il nome invariabile del provider utilizzato per ottenere un'istanza della classe DbProviderFactory. Il valore predefinito è SqlClient. |

## Esempi

Mostra come leggere un progetto da un file XML Primavera con più progetti utilizzando un nome provider.

```csharp
var connectionString = "Data Source=" + DataDir + "\\PPMDBSQLite.db";

// Crea le impostazioni DB Primavera usando la stringa di connessione e l'ID del progetto
var settings = new PrimaveraDbSettings(connectionString, 4502);
settings.ProviderInvariantName = "System.Data.SQLite";

Console.WriteLine("Connection String: " + settings.ConnectionString);
Console.WriteLine("Provider Name: " + settings.ProviderInvariantName);

var project = new Project(settings);
project.Save(OutDir + "SupportForSQLiteDatabase_out.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


