---
title: "Klasse MpdSettings"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Connectivity.MpdSettings class. Stelt u in staat om de benodigde opties in te stellen om projectgegevens te lezen uit een MPD-formaat MS Access-databasebestand"
type: docs
weight: 300
url: /nl/net/aspose.tasks.connectivity/mpdsettings/
---
## MpdSettings class

Staat toe om de benodigde opties in te stellen om projectgegevens te lezen uit het MPD‑formaat (MS Access‑databasebestandformaat).

```csharp
public class MpdSettings : DbSettings
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [MpdSettings](mpdsettings/)(string, int) | Initialiseert een nieuw exemplaar van de `MpdSettings` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Haalt op of stelt de verbindingsreeks in. |
| [ProjectId](../../aspose.tasks.connectivity/mpdsettings/projectid/) { get; } | Haalt de ID van het te lezen project op. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Haalt op of stelt de callback in die wordt aangeroepen tijdens projectlaadbewerkingen. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Haalt op of stelt een instantie van DbProviderFactory in die wordt gebruikt om verbinding te maken met de database. Als zowel ProviderFactory als ProviderInvariantName zijn ingesteld, heeft ProviderFactory prioriteit. Standaardwaarde is null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Haalt op of stelt de provider-invariante naam in die wordt gebruikt om een instantie van de DbProviderFactory klasse te verkrijgen. Standaardwaarde is SqlClient. |

## Voorbeelden

Toont hoe MPD-instellingen te gebruiken om de import van een project uit de database te beheersen.

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Zie ook

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


