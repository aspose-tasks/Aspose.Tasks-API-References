---
title: "MpdSettings.ProjectId"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "MpdSettings eigenschap. Haalt de id van het project op om te lezen"
type: docs
weight: 20
url: /nl/net/aspose.tasks.connectivity/mpdsettings/projectid/
---
## MpdSettings.ProjectId property

Haalt de ID van het te lezen project op.

```csharp
public int ProjectId { get; }
```

## Voorbeelden

Toont hoe MPD-instellingen te gebruiken om de import van een project uit de database te beheersen.

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Zie ook

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


