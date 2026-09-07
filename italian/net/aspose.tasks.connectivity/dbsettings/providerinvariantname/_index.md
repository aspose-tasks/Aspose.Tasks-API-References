---
title: "DbSettings.ProviderInvariantName"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà DbSettings. Ottiene o imposta il nome invariabile del provider che è usato per ottenere un'istanza della classe DbProviderFactory. Il valore predefinito è SqlClient."
type: docs
weight: 40
url: /it/net/aspose.tasks.connectivity/dbsettings/providerinvariantname/
---
## DbSettings.ProviderInvariantName property

Ottiene o imposta il nome invariabile del provider utilizzato per ottenere un'istanza della classe DbProviderFactory. Il valore predefinito è SqlClient.

```csharp
public string ProviderInvariantName { get; set; }
```

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

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


