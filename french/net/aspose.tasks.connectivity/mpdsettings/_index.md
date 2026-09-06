---
title: "Classe MpdSettings"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Connectivity.MpdSettings. Permet de définir les options nécessaires pour lire les données du projet à partir du format MPD du fichier de base de données MS Access"
type: docs
weight: 300
url: /fr/net/aspose.tasks.connectivity/mpdsettings/
---
## MpdSettings class

Permet de définir les options nécessaires pour lire les données du projet au format MPD (format de fichier de base de données MS Access).

```csharp
public class MpdSettings : DbSettings
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [MpdSettings](mpdsettings/)(string, int) | Initialise une nouvelle instance de la classe `MpdSettings`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Obtient ou définit la chaîne de connexion. |
| [ProjectId](../../aspose.tasks.connectivity/mpdsettings/projectid/) { get; } | Obtient l'identifiant du projet à lire. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Obtient ou définit le rappel à invoquer pendant les opérations de chargement du projet. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Obtient ou définit une instance de DbProviderFactory utilisée pour se connecter à la base de données. Si ProviderFactory et ProviderInvariantName sont tous deux définis, ProviderFactory a la priorité. La valeur par défaut est null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Obtient ou définit le nom invariant du fournisseur utilisé pour obtenir une instance de la classe DbProviderFactory. La valeur par défaut est SqlClient. |

## Exemples

Montre comment utiliser les paramètres MPD pour contrôler l'importation du projet depuis la base de données.

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Voir aussi

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


