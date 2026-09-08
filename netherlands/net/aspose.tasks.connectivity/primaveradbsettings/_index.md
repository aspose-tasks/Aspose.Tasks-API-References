---
title: "Klasse PrimaveraDbSettings"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Connectivity.PrimaveraDbSettings class. Stelt u in staat om de benodigde opties in te stellen om projectgegevens te lezen uit een Primavera-database"
type: docs
weight: 320
url: /nl/net/aspose.tasks.connectivity/primaveradbsettings/
---
## PrimaveraDbSettings class

Staat toe om de benodigde opties in te stellen om projectgegevens te lezen uit de Primavera‑database.

```csharp
public class PrimaveraDbSettings : DbSettings
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [PrimaveraDbSettings](primaveradbsettings/)(string, int) | Initialiseert een nieuw exemplaar van de `PrimaveraDbSettings` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Haalt op of stelt de verbindingsreeks in. |
| [ProjectId](../../aspose.tasks.connectivity/primaveradbsettings/projectid/) { get; } | Haalt de ID van het te lezen project op. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Haalt op of stelt de callback in die wordt aangeroepen tijdens projectlaadbewerkingen. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Haalt op of stelt een instantie van DbProviderFactory in die wordt gebruikt om verbinding te maken met de database. Als zowel ProviderFactory als ProviderInvariantName zijn ingesteld, heeft ProviderFactory prioriteit. Standaardwaarde is null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Haalt op of stelt de provider-invariante naam in die wordt gebruikt om een instantie van de DbProviderFactory klasse te verkrijgen. Standaardwaarde is SqlClient. |

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

Toont hoe je beknopte informatie over projecten uit een Primavera-database kunt ophalen.

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

### Zie ook

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


