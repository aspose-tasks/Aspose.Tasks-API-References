---
title: "DbSettings.ProviderFactory"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété DbSettings. Obtient ou définit une instance de DbProviderFactory qui est utilisée pour se connecter à la base de données. Si ProviderFactory et ProviderInvariantName sont tous deux définis, ProviderFactory a la priorité. La valeur par défaut est null"
type: docs
weight: 30
url: /fr/net/aspose.tasks.connectivity/dbsettings/providerfactory/
---
## DbSettings.ProviderFactory property

Obtient ou définit une instance de DbProviderFactory utilisée pour se connecter à la base de données. Si ProviderFactory et ProviderInvariantName sont tous deux définis, ProviderFactory a la priorité. La valeur par défaut est null.

```csharp
public DbProviderFactory ProviderFactory { get; set; }
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

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


