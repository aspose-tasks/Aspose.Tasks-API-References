---
title: "DbSettings.ProviderFactory"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "DbSettings eigenschap. Haalt op of stelt een instantie van DbProviderFactory in die wordt gebruikt om verbinding te maken met de database. Als zowel ProviderFactory als ProviderInvariantName zijn ingesteld, heeft ProviderFactory prioriteit. Standaardwaarde is null."
type: docs
weight: 30
url: /nl/net/aspose.tasks.connectivity/dbsettings/providerfactory/
---
## DbSettings.ProviderFactory property

Haalt op of stelt een instantie van DbProviderFactory in die wordt gebruikt om verbinding te maken met de database. Als zowel ProviderFactory als ProviderInvariantName zijn ingesteld, heeft ProviderFactory prioriteit. Standaardwaarde is null.

```csharp
public DbProviderFactory ProviderFactory { get; set; }
```

## Voorbeelden

Toont hoe een project uit een Primavera-database te importeren.

```csharp
// Initialiseer een nieuw exemplaar van de PrimaveraDbSettings klasse met verbindingsreeks en project-ID
var settings = new PrimaveraDbSettings(GetConnectionString(), 4502);
settings.ProviderFactory = SqliteFactory.Instance;

Console.WriteLine("Project UID to read: " + settings.ProjectId);

// lees het project met UID = 4502
var project = new Project(settings);
Console.WriteLine(project.Uid);
Console.WriteLine(project.Name);
Console.WriteLine(project.PrimaveraProperties.ShortName);
```

### Zie ook

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


