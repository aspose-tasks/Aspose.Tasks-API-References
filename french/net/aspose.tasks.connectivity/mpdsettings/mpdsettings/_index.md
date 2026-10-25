---
title: "MpdSettings.MpdSettings"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur MpdSettings. Initialise une nouvelle instance de la classe MpdSettings"
type: docs
weight: 10
url: /fr/net/aspose.tasks.connectivity/mpdsettings/mpdsettings/
---
## MpdSettings constructor

Initialise une nouvelle instance de la classe [`MpdSettings`](../).

```csharp
public MpdSettings(string connectionString, int projectId)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| connectionString | Chaîne | la chaîne de connexion spécifiée. |
| projectId | Int32 | l'identifiant spécifié d'un projet à lire. |

## Exemples

Montre comment lire un projet à partir d'un fichier MPD.

```csharp
DbSettings settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Voir aussi

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


