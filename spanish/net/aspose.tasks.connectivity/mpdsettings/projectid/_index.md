---
title: "MpdSettings.ProjectId"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad MpdSettings. Obtiene el id del proyecto para leer."
type: docs
weight: 20
url: /es/net/aspose.tasks.connectivity/mpdsettings/projectid/
---
## MpdSettings.ProjectId property

Obtiene el ID del proyecto a leer.

```csharp
public int ProjectId { get; }
```

## Ejemplos

Muestra cómo usar la configuración MPD para controlar la importación del proyecto desde la base de datos.

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Ver también

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


