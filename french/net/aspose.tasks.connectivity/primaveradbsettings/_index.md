---
title: "Classe PrimaveraDbSettings"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Connectivity.PrimaveraDbSettings. Permet de définir les options nécessaires pour lire les données du projet à partir de la base de données Primavera"
type: docs
weight: 320
url: /fr/net/aspose.tasks.connectivity/primaveradbsettings/
---
## PrimaveraDbSettings class

Permet de définir les options nécessaires pour lire les données du projet à partir de la base de données Primavera.

```csharp
public class PrimaveraDbSettings : DbSettings
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PrimaveraDbSettings](primaveradbsettings/)(string, int) | Initialise une nouvelle instance de la classe `PrimaveraDbSettings`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Obtient ou définit la chaîne de connexion. |
| [ProjectId](../../aspose.tasks.connectivity/primaveradbsettings/projectid/) { get; } | Obtient l'identifiant du projet à lire. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Obtient ou définit le rappel à invoquer pendant les opérations de chargement du projet. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Obtient ou définit une instance de DbProviderFactory utilisée pour se connecter à la base de données. Si ProviderFactory et ProviderInvariantName sont tous deux définis, ProviderFactory a la priorité. La valeur par défaut est null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Obtient ou définit le nom invariant du fournisseur utilisé pour obtenir une instance de la classe DbProviderFactory. La valeur par défaut est SqlClient. |

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

Montre comment obtenir des informations brèves des projets à partir d'une base de données Primavera.

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

### Voir aussi

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


