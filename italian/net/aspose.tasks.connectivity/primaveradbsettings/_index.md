---
title: "Classe PrimaveraDbSettings"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Connectivity.PrimaveraDbSettings. Consente di impostare le opzioni necessarie per leggere i dati del progetto dal database Primavera"
type: docs
weight: 320
url: /it/net/aspose.tasks.connectivity/primaveradbsettings/
---
## PrimaveraDbSettings class

Consente di impostare le opzioni necessarie per leggere i dati del progetto dal database Primavera.

```csharp
public class PrimaveraDbSettings : DbSettings
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PrimaveraDbSettings](primaveradbsettings/)(string, int) | Inizializza una nuova istanza della classe `PrimaveraDbSettings`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Ottiene o imposta la stringa di connessione. |
| [ProjectId](../../aspose.tasks.connectivity/primaveradbsettings/projectid/) { get; } | Ottiene l'ID del progetto da leggere. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Ottiene o imposta la callback da invocare durante le operazioni di caricamento del progetto. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Ottiene o imposta un'istanza di DbProviderFactory utilizzata per connettersi al DB. Se sia ProviderFactory sia ProviderInvariantName sono impostati, ProviderFactory ha la priorità. Il valore predefinito è null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Ottiene o imposta il nome invariabile del provider utilizzato per ottenere un'istanza della classe DbProviderFactory. Il valore predefinito è SqlClient. |

## Esempi

Mostra come importare un progetto da un database Primavera.

```csharp
// Inizializza una nuova istanza della classe PrimaveraDbSettings con la stringa di connessione e l'ID del progetto
var settings = new PrimaveraDbSettings(GetConnectionString(), 4502);
settings.ProviderFactory = SqliteFactory.Instance;

Console.WriteLine("Project UID to read: " + settings.ProjectId);

// leggi il progetto con UID = 4502
var project = new Project(settings);
Console.WriteLine(project.Uid);
Console.WriteLine(project.Name);
Console.WriteLine(project.PrimaveraProperties.ShortName);
```

Mostra come ottenere informazioni brevi sui progetti da un database Primavera.

```csharp
var settings = new PrimaveraDbSettings(GetConnectionString(), 0);

var reader = new PrimaveraDbReader(settings);
var projectInfos = reader.GetProjectInfos();

foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - '{2}'", info.Uid, info.ShortName, info.Name);
}

var firstProject = reader.LoadProject(projectInfos[0].Uid);
Console.WriteLine(firstProject.Uid);
Console.WriteLine(firstProject.Name);
Console.WriteLine(firstProject.PrimaveraProperties.ShortName);
```

### Vedi anche

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


