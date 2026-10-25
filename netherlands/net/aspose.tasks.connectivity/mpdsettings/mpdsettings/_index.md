---
title: "MpdSettings.MpdSettings"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "MpdSettings constructor. Initialiseert een nieuw exemplaar van de MpdSettings-klasse"
type: docs
weight: 10
url: /nl/net/aspose.tasks.connectivity/mpdsettings/mpdsettings/
---
## MpdSettings constructor

Initialiseert een nieuw exemplaar van de [`MpdSettings`](../) klasse.

```csharp
public MpdSettings(string connectionString, int projectId)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| connectionString | String | de opgegeven connection string. |
| projectId | Int32 | de opgegeven id van een project om te lezen. |

## Voorbeelden

Toont hoe een project uit een MPD-bestand te lezen.

```csharp
DbSettings settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Zie ook

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


