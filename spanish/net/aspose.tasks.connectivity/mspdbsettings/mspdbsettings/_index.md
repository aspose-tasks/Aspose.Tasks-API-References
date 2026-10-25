---
title: "MspDbSettings.MspDbSettings"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor de MspDbSettings. Inicializa una nueva instancia de la clase MspDbSettings"
type: docs
weight: 10
url: /es/net/aspose.tasks.connectivity/mspdbsettings/mspdbsettings/
---
## MspDbSettings constructor

Inicializa una nueva instancia de la clase [`MspDbSettings`](../).

```csharp
public MspDbSettings(string connectionString, Guid projectGuid)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| connectionString | Cadena | la cadena de conexión especificada. |
| projectGuid | Guid | el GUID especificado de un proyecto para leer. |

## Ejemplos

Muestra cómo importar un proyecto desde una base de datos.

```csharp
try
{
    // Crear cadena de conexión
    var connectionString = new SqlConnectionStringBuilder();
    connectionString.DataSource = "192.168.56.2,1433";
    connectionString.Encrypt = true;
    connectionString.TrustServerCertificate = true;
    connectionString.InitialCatalog = "ProjectServer_Published";
    connectionString.NetworkLibrary = "DBMSSOCN";
    connectionString.UserID = "sa";
    connectionString.Password = "*****";

    // crear configuraciones para cargar desde la base de datos de MS
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

### Ver también

* class [MspDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mspdbsettings/)
* assembly [Aspose.Tasks](../../../)


