---
title: "Classe DbSettings"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Connectivity.DbSettings. Permet de spécifier les paramètres pour lire depuis la base de données du projet"
type: docs
weight: 290
url: /fr/net/aspose.tasks.connectivity/dbsettings/
---
## DbSettings class

Permet de spécifier les paramètres pour lire à partir de la base de données du projet.

```csharp
public abstract class DbSettings
```

## Propriétés

| Nom | Description |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Obtient ou définit la chaîne de connexion. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Obtient ou définit le rappel à invoquer pendant les opérations de chargement du projet. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Obtient ou définit une instance de DbProviderFactory utilisée pour se connecter à la base de données. Si ProviderFactory et ProviderInvariantName sont tous deux définis, ProviderFactory a la priorité. La valeur par défaut est null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Obtient ou définit le nom invariant du fournisseur utilisé pour obtenir une instance de la classe DbProviderFactory. La valeur par défaut est SqlClient. |

## Exemples

Montre comment lire un projet à partir d'un fichier XML Primavera contenant plusieurs projets en utilisant le nom d'un fournisseur.

```csharp
var connectionString = "Data Source=" + DataDir + "\\PPMDBSQLite.db";

// Créer les paramètres de la base de données Primavera en utilisant la chaîne de connexion et l'identifiant du projet
var settings = new PrimaveraDbSettings(connectionString, 4502);
settings.ProviderInvariantName = "System.Data.SQLite";

Console.WriteLine("Connection String: " + settings.ConnectionString);
Console.WriteLine("Provider Name: " + settings.ProviderInvariantName);

var project = new Project(settings);
project.Save(OutDir + "SupportForSQLiteDatabase_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


