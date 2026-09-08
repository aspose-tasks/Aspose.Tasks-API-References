---
title: "PrimaveraDbSettings.PrimaveraDbSettings"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PrimaveraDbSettings constructor. Initialiseert een nieuwe instantie van de PrimaveraDbSettings klasse."
type: docs
weight: 10
url: /nl/net/aspose.tasks.connectivity/primaveradbsettings/primaveradbsettings/
---
## PrimaveraDbSettings constructor

Initialiseert een nieuwe instantie van de [`PrimaveraDbSettings`](../) klasse.

```csharp
public PrimaveraDbSettings(string connectionString, int projectId)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| connectionString | String | de opgegeven connection string. |
| projectId | Int32 | de opgegeven id van een project om te lezen. |

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

* class [PrimaveraDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../primaveradbsettings/)
* assembly [Aspose.Tasks](../../../)


