---
title: MspDbSettings.Schema
second_title: Aspose.Tasks for .NET API Reference
description: MspDbSettings property. Gets or sets the schema of the MS Project Server. The default value is pub
type: docs
weight: 30
url: /net/aspose.tasks.connectivity/mspdbsettings/schema/
---
## MspDbSettings.Schema property

Gets or sets the schema of the MS Project Server. The default value is "pub".

```csharp
public string Schema { get; set; }
```

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

* class [MspDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mspdbsettings/)
* assembly [Aspose.Tasks](../../../)


