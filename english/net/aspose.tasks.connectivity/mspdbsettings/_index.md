---
title: Class MspDbSettings
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Connectivity.MspDbSettings class. Allows to set necessary options to read project data from MS Project Server database
type: docs
weight: 310
url: /net/aspose.tasks.connectivity/mspdbsettings/
---
## MspDbSettings class

Allows to set necessary options to read project data from MS Project Server database.

```csharp
public class MspDbSettings : DbSettings
```

## Constructors

| Name | Description |
| --- | --- |
| [MspDbSettings](mspdbsettings/)(string, Guid) | Initializes a new instance of the `MspDbSettings` class. |

## Properties

| Name | Description |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Gets or sets the connection string. |
| [ProjectGuid](../../aspose.tasks.connectivity/mspdbsettings/projectguid/) { get; } | Gets the guid of the project to read. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Gets or sets provider invariant name which is used to get an instance of the DbProviderFactory class. Default value is SqlClient. |
| [Schema](../../aspose.tasks.connectivity/mspdbsettings/schema/) { get; set; } | Gets or sets the schema of the MS Project Server. The default value is "pub". |

## Examples

Shows how to import a project from a database.

```csharp
try
{
    // Create connection string
    var connectionString = new SqlConnectionStringBuilder();
    connectionString.DataSource = "192.168.56.2,1433";
    connectionString.Encrypt = true;
    connectionString.TrustServerCertificate = true;
    connectionString.InitialCatalog = "ProjectServer_Published";
    connectionString.NetworkLibrary = "DBMSSOCN";
    connectionString.UserID = "sa";
    connectionString.Password = "*****";

    // create settings to load from MS database
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

### See Also

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


