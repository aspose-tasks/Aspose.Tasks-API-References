---
title: "DbSettings.ConnectionString"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété DbSettings. Obtient ou définit la chaîne de connexion"
type: docs
weight: 10
url: /fr/net/aspose.tasks.connectivity/dbsettings/connectionstring/
---
## DbSettings.ConnectionString property

Obtient ou définit la chaîne de connexion.

```csharp
public string ConnectionString { get; set; }
```

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

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


