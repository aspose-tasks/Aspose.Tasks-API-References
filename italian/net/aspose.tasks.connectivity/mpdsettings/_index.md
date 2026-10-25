---
title: "Classe MpdSettings"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Connectivity.MpdSettings. Consente di impostare le opzioni necessarie per leggere i dati del progetto dal formato MPD del file di database MS Access"
type: docs
weight: 300
url: /it/net/aspose.tasks.connectivity/mpdsettings/
---
## MpdSettings class

Consente di impostare le opzioni necessarie per leggere i dati del progetto dal formato MPD (formato file del database MS Access).

```csharp
public class MpdSettings : DbSettings
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [MpdSettings](mpdsettings/)(string, int) | Inizializza una nuova istanza della classe `MpdSettings`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Ottiene o imposta la stringa di connessione. |
| [ProjectId](../../aspose.tasks.connectivity/mpdsettings/projectid/) { get; } | Ottiene l'ID del progetto da leggere. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Ottiene o imposta la callback da invocare durante le operazioni di caricamento del progetto. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Ottiene o imposta un'istanza di DbProviderFactory utilizzata per connettersi al DB. Se sia ProviderFactory sia ProviderInvariantName sono impostati, ProviderFactory ha la priorità. Il valore predefinito è null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Ottiene o imposta il nome invariabile del provider utilizzato per ottenere un'istanza della classe DbProviderFactory. Il valore predefinito è SqlClient. |

## Esempi

Mostra come utilizzare le impostazioni MPD per controllare l'importazione del progetto dal database.

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Vedi anche

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


