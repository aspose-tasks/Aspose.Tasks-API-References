---
title: "PrimaveraDbSettings.PrimaveraDbSettings"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor de PrimaveraDbSettings. Inicializa una nueva instancia de la clase PrimaveraDbSettings"
type: docs
weight: 10
url: /es/net/aspose.tasks.connectivity/primaveradbsettings/primaveradbsettings/
---
## PrimaveraDbSettings constructor

Inicializa una nueva instancia de la clase [`PrimaveraDbSettings`](../).

```csharp
public PrimaveraDbSettings(string connectionString, int projectId)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| connectionString | Cadena | la cadena de conexión especificada. |
| projectId | Int32 | el id especificado de un proyecto para leer. |

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

### Ver también

* class [PrimaveraDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../primaveradbsettings/)
* assembly [Aspose.Tasks](../../../)


