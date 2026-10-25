---
title: "MpdSettings.ProjectId"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà MpdSettings. Ottiene l'id del progetto da leggere."
type: docs
weight: 20
url: /it/net/aspose.tasks.connectivity/mpdsettings/projectid/
---
## MpdSettings.ProjectId property

Ottiene l'ID del progetto da leggere.

```csharp
public int ProjectId { get; }
```

## Esempi

Mostra come utilizzare le impostazioni MPD per controllare l'importazione del progetto dal database.

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Vedi anche

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


