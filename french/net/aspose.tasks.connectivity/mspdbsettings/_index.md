---
title: "Classe MspDbSettings"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Connectivity.MspDbSettings. Permet de définir les options nécessaires pour lire les données du projet à partir de la base de données MS Project Server"
type: docs
weight: 310
url: /fr/net/aspose.tasks.connectivity/mspdbsettings/
---
## MspDbSettings class

Permet de définir les options nécessaires pour lire les données du projet à partir de la base de données MS Project Server.

```csharp
public class MspDbSettings : DbSettings
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [MspDbSettings](mspdbsettings/)(string, Guid) | Initialise une nouvelle instance de la classe `MspDbSettings`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Obtient ou définit la chaîne de connexion. |
| [ProjectGuid](../../aspose.tasks.connectivity/mspdbsettings/projectguid/) { get; } | Obtient le GUID du projet à lire. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Obtient ou définit le rappel à invoquer pendant les opérations de chargement du projet. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Obtient ou définit une instance de DbProviderFactory utilisée pour se connecter à la base de données. Si ProviderFactory et ProviderInvariantName sont tous deux définis, ProviderFactory a la priorité. La valeur par défaut est null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Obtient ou définit le nom invariant du fournisseur utilisé pour obtenir une instance de la classe DbProviderFactory. La valeur par défaut est SqlClient. |
| [Schema](../../aspose.tasks.connectivity/mspdbsettings/schema/) { get; set; } | Obtient ou définit le schéma du MS Project Server. La valeur par défaut est "pub". |

## Exemples

Montre comment importer un projet depuis une base de données.

```csharp
try
{
    // Créer une chaîne de connexion
    var connectionString = new SqlConnectionStringBuilder();
    connectionString.DataSource = "192.168.56.2,1433";
    connectionString.Encrypt = true;
    connectionString.TrustServerCertificate = true;
    connectionString.InitialCatalog = "ProjectServer_Published";
    connectionString.NetworkLibrary = "DBMSSOCN";
    connectionString.UserID = "sa";
    connectionString.Password = "*****";

    // créer des paramètres pour charger depuis la base de données MS
    var settings = new MspDbSettings(connectionString.ConnectionString, new Guid("E6426C44-D6CB-4B9C-AF16-48910ACE0F54"));
    settings.Schema = "dbo";

    Console.WriteLine("Project GUID to load: " + settings.ProjectGuid);

    var project = new Project(settings);

    project.Save(OutDir + "ImportProjectDataFromDatabase_out.mpp", SaveFileFormat.Mpp);
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message + " Please setup proper data source (DataSource, InitialCatalog etc)");
}
```

### Voir aussi

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


