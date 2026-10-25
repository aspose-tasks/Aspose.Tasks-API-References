---
title: "MspDbSettings.Schema"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété MspDbSettings. Obtient ou définit le schéma du serveur MS Project. La valeur par défaut est pub"
type: docs
weight: 30
url: /fr/net/aspose.tasks.connectivity/mspdbsettings/schema/
---
## MspDbSettings.Schema property

Obtient ou définit le schéma du MS Project Server. La valeur par défaut est "pub".

```csharp
public string Schema { get; set; }
```

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

* class [MspDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mspdbsettings/)
* assembly [Aspose.Tasks](../../../)


