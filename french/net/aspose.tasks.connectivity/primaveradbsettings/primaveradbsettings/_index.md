---
title: "PrimaveraDbSettings.PrimaveraDbSettings"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur PrimaveraDbSettings. Initialise une nouvelle instance de la classe PrimaveraDbSettings"
type: docs
weight: 10
url: /fr/net/aspose.tasks.connectivity/primaveradbsettings/primaveradbsettings/
---
## PrimaveraDbSettings constructor

Initialise une nouvelle instance de la classe [`PrimaveraDbSettings`](../).

```csharp
public PrimaveraDbSettings(string connectionString, int projectId)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| connectionString | Chaîne | la chaîne de connexion spécifiée. |
| projectId | Int32 | l'identifiant spécifié d'un projet à lire. |

## Exemples

Montre comment importer un projet depuis une base de données Primavera.

```csharp
// Initialiser une nouvelle instance de la classe PrimaveraDbSettings avec la chaîne de connexion et l'identifiant du projet
var settings = new PrimaveraDbSettings(GetConnectionString(), 4502);
settings.ProviderFactory = SqliteFactory.Instance;

Console.WriteLine("Project UID to read: " + settings.ProjectId);

// Lire le projet avec UID = 4502
var project = new Project(settings);
Console.WriteLine(project.Uid);
Console.WriteLine(project.Name);
Console.WriteLine(project.PrimaveraProperties.ShortName);
```

### Voir aussi

* class [PrimaveraDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../primaveradbsettings/)
* assembly [Aspose.Tasks](../../../)


