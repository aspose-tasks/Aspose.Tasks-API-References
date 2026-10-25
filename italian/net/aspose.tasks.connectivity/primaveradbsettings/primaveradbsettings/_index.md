---
title: "PrimaveraDbSettings.PrimaveraDbSettings"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore PrimaveraDbSettings. Inizializza una nuova istanza della classe PrimaveraDbSettings"
type: docs
weight: 10
url: /it/net/aspose.tasks.connectivity/primaveradbsettings/primaveradbsettings/
---
## PrimaveraDbSettings constructor

Inizializza una nuova istanza della classe [`PrimaveraDbSettings`](../).

```csharp
public PrimaveraDbSettings(string connectionString, int projectId)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| connectionString | Stringa | la stringa di connessione specificata. |
| projectId | Int32 | l'id specificato di un progetto da leggere. |

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

### Vedi anche

* class [PrimaveraDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../primaveradbsettings/)
* assembly [Aspose.Tasks](../../../)


