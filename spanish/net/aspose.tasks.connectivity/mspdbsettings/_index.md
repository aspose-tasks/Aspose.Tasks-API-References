---
title: "Clase MspDbSettings"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Connectivity.MspDbSettings. Permite establecer las opciones necesarias para leer datos del proyecto desde la base de datos de MS Project Server"
type: docs
weight: 310
url: /es/net/aspose.tasks.connectivity/mspdbsettings/
---
## MspDbSettings class

Permite establecer opciones necesarias para leer datos del proyecto desde la base de datos de MS Project Server.

```csharp
public class MspDbSettings : DbSettings
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [MspDbSettings](mspdbsettings/)(string, Guid) | Inicializa una nueva instancia de la clase `MspDbSettings`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Obtiene o establece la cadena de conexión. |
| [ProjectGuid](../../aspose.tasks.connectivity/mspdbsettings/projectguid/) { get; } | Obtiene el GUID del proyecto a leer. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Obtiene o establece la función de devolución de llamada que se invocará durante las operaciones de carga del proyecto. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Obtiene o establece una instancia de DbProviderFactory que se utiliza para conectar a la base de datos. Si se establecen tanto ProviderFactory como ProviderInvariantName, ProviderFactory tiene prioridad. El valor predeterminado es null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Obtiene o establece el nombre invariante del proveedor que se usa para obtener una instancia de la clase DbProviderFactory. El valor predeterminado es SqlClient. |
| [Schema](../../aspose.tasks.connectivity/mspdbsettings/schema/) { get; set; } | Obtiene o establece el esquema del MS Project Server. El valor predeterminado es \"pub\". |

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

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


