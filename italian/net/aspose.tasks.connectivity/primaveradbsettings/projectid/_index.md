---
title: "PrimaveraDbSettings.ProjectId"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà PrimaveraDbSettings. Ottiene l'ID del progetto da leggere"
type: docs
weight: 20
url: /it/net/aspose.tasks.connectivity/primaveradbsettings/projectid/
---
## PrimaveraDbSettings.ProjectId property

Ottiene l'ID del progetto da leggere.

```csharp
public int ProjectId { get; }
```

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


