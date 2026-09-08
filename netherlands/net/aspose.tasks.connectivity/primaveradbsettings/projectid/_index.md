---
title: "PrimaveraDbSettings.ProjectId"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PrimaveraDbSettings eigenschap. Haalt de id van het project op dat gelezen moet worden."
type: docs
weight: 20
url: /nl/net/aspose.tasks.connectivity/primaveradbsettings/projectid/
---
## PrimaveraDbSettings.ProjectId property

Haalt de ID van het te lezen project op.

```csharp
public int ProjectId { get; }
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

* class [PrimaveraDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../primaveradbsettings/)
* assembly [Aspose.Tasks](../../../)


