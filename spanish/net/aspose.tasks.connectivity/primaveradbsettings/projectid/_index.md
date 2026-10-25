---
title: "PrimaveraDbSettings.ProjectId"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PrimaveraDbSettings. Obtiene el id del proyecto a leer"
type: docs
weight: 20
url: /es/net/aspose.tasks.connectivity/primaveradbsettings/projectid/
---
## PrimaveraDbSettings.ProjectId property

Obtiene el ID del proyecto a leer.

```csharp
public int ProjectId { get; }
```

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


