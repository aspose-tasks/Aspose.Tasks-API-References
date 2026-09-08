---
title: "Clase DbSettings"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Connectivity.DbSettings. Permite especificar configuraciones para leer desde la base de datos del proyecto"
type: docs
weight: 290
url: /es/net/aspose.tasks.connectivity/dbsettings/
---
## DbSettings class

Permite especificar configuraciones para leer de la base de datos del proyecto.

```csharp
public abstract class DbSettings
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Obtiene o establece la cadena de conexión. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Obtiene o establece la función de devolución de llamada que se invocará durante las operaciones de carga del proyecto. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Obtiene o establece una instancia de DbProviderFactory que se utiliza para conectar a la base de datos. Si se establecen tanto ProviderFactory como ProviderInvariantName, ProviderFactory tiene prioridad. El valor predeterminado es null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Obtiene o establece el nombre invariante del proveedor que se usa para obtener una instancia de la clase DbProviderFactory. El valor predeterminado es SqlClient. |

## Ejemplos

Muestra cómo leer un proyecto desde un archivo XML de Primavera con múltiples proyectos usando un nombre de proveedor.

```csharp
var connectionString = "Data Source=" + DataDir + "\\PPMDBSQLite.db";

// Crear configuraciones de DB de Primavera usando la cadena de conexión y el ID del proyecto
var settings = new PrimaveraDbSettings(connectionString, 4502);
settings.ProviderInvariantName = "System.Data.SQLite";

Console.WriteLine("Connection String: " + settings.ConnectionString);
Console.WriteLine("Provider Name: " + settings.ProviderInvariantName);

var project = new Project(settings);
project.Save(OutDir + "SupportForSQLiteDatabase_out.mpp", SaveFileFormat.Mpp);
```

### Ver también

* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


