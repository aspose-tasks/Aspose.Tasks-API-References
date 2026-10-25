---
title: "Clase PrimaveraDbSettings"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Connectivity.PrimaveraDbSettings. Permite establecer las opciones necesarias para leer datos del proyecto desde la base de datos de Primavera"
type: docs
weight: 320
url: /es/net/aspose.tasks.connectivity/primaveradbsettings/
---
## PrimaveraDbSettings class

Permite establecer opciones necesarias para leer datos del proyecto desde la base de datos de Primavera.

```csharp
public class PrimaveraDbSettings : DbSettings
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PrimaveraDbSettings](primaveradbsettings/)(string, int) | Inicializa una nueva instancia de la clase `PrimaveraDbSettings`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Obtiene o establece la cadena de conexión. |
| [ProjectId](../../aspose.tasks.connectivity/primaveradbsettings/projectid/) { get; } | Obtiene el ID del proyecto a leer. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Obtiene o establece la función de devolución de llamada que se invocará durante las operaciones de carga del proyecto. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Obtiene o establece una instancia de DbProviderFactory que se utiliza para conectar a la base de datos. Si se establecen tanto ProviderFactory como ProviderInvariantName, ProviderFactory tiene prioridad. El valor predeterminado es null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Obtiene o establece el nombre invariante del proveedor que se usa para obtener una instancia de la clase DbProviderFactory. El valor predeterminado es SqlClient. |

## Ejemplos

Muestra cómo importar un proyecto desde una base de datos de Primavera.

```csharp
// Inicializa una nueva instancia de la clase PrimaveraDbSettings con la cadena de conexión y el ID del proyecto
var settings = new PrimaveraDbSettings(GetConnectionString(), 4502);
settings.ProviderFactory = SqliteFactory.Instance;

Console.WriteLine("Project UID to read: " + settings.ProjectId);

// lee el proyecto con UID = 4502
var project = new Project(settings);
Console.WriteLine(project.Uid);
Console.WriteLine(project.Name);
Console.WriteLine(project.PrimaveraProperties.ShortName);
```

Muestra cómo obtener información breve de los proyectos desde una base de datos Primavera.

```csharp
var settings = new PrimaveraDbSettings(GetConnectionString(), 0);

var reader = new PrimaveraDbReader(settings);
var projectInfos = reader.GetProjectInfos();

foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - '{2}'", info.Uid, info.ShortName, info.Name);
}

var firstProject = reader.LoadProject(projectInfos[0].Uid);
Console.WriteLine(firstProject.Uid);
Console.WriteLine(firstProject.Name);
Console.WriteLine(firstProject.PrimaveraProperties.ShortName);
```

### Ver también

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


