---
title: "DbSettings.ProviderFactory"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad DbSettings. Obtiene o establece una instancia de DbProviderFactory que se utiliza para conectar a la base de datos. Si tanto ProviderFactory como ProviderInvariantName están configurados, ProviderFactory tiene prioridad. El valor predeterminado es null"
type: docs
weight: 30
url: /es/net/aspose.tasks.connectivity/dbsettings/providerfactory/
---
## DbSettings.ProviderFactory property

Obtiene o establece una instancia de DbProviderFactory que se utiliza para conectar a la base de datos. Si se establecen tanto ProviderFactory como ProviderInvariantName, ProviderFactory tiene prioridad. El valor predeterminado es null.

```csharp
public DbProviderFactory ProviderFactory { get; set; }
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

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


