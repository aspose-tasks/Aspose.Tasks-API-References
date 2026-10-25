---
title: "PrimaveraDbSettings.ProjectId"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PrimaveraDbSettings. Obtient l'identifiant du projet à lire"
type: docs
weight: 20
url: /fr/net/aspose.tasks.connectivity/primaveradbsettings/projectid/
---
## PrimaveraDbSettings.ProjectId property

Obtient l'identifiant du projet à lire.

```csharp
public int ProjectId { get; }
```

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


