---
title: "Clase MpdSettings"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Connectivity.MpdSettings. Permite establecer las opciones necesarias para leer datos del proyecto desde el formato MPD de archivo de base de datos MS Access"
type: docs
weight: 300
url: /es/net/aspose.tasks.connectivity/mpdsettings/
---
## MpdSettings class

Permite establecer opciones necesarias para leer datos del proyecto desde el formato MPD (formato de archivo de base de datos MS Access).

```csharp
public class MpdSettings : DbSettings
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [MpdSettings](mpdsettings/)(string, int) | Inicializa una nueva instancia de la clase `MpdSettings`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Obtiene o establece la cadena de conexión. |
| [ProjectId](../../aspose.tasks.connectivity/mpdsettings/projectid/) { get; } | Obtiene el ID del proyecto a leer. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Obtiene o establece la función de devolución de llamada que se invocará durante las operaciones de carga del proyecto. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Obtiene o establece una instancia de DbProviderFactory que se utiliza para conectar a la base de datos. Si se establecen tanto ProviderFactory como ProviderInvariantName, ProviderFactory tiene prioridad. El valor predeterminado es null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Obtiene o establece el nombre invariante del proveedor que se usa para obtener una instancia de la clase DbProviderFactory. El valor predeterminado es SqlClient. |

## Ejemplos

Muestra cómo usar la configuración MPD para controlar la importación del proyecto desde la base de datos.

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Ver también

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


