---
title: "MpdSettings.ProjectId"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété MpdSettings. Obtient l'identifiant du projet à lire"
type: docs
weight: 20
url: /fr/net/aspose.tasks.connectivity/mpdsettings/projectid/
---
## MpdSettings.ProjectId property

Obtient l'identifiant du projet à lire.

```csharp
public int ProjectId { get; }
```

## Exemples

Montre comment utiliser les paramètres MPD pour contrôler l'importation du projet depuis la base de données.

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Voir aussi

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


