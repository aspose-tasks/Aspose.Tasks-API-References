---
title: "DbSettings.ProviderFactory"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà DbSettings. Ottiene o imposta un'istanza di DbProviderFactory che viene utilizzata per connettersi al DB. Se sia ProviderFactory sia ProviderInvariantName sono impostati, ProviderFactory ha la priorità. Il valore predefinito è null"
type: docs
weight: 30
url: /it/net/aspose.tasks.connectivity/dbsettings/providerfactory/
---
## DbSettings.ProviderFactory property

Ottiene o imposta un'istanza di DbProviderFactory utilizzata per connettersi al DB. Se sia ProviderFactory sia ProviderInvariantName sono impostati, ProviderFactory ha la priorità. Il valore predefinito è null.

```csharp
public DbProviderFactory ProviderFactory { get; set; }
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

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


