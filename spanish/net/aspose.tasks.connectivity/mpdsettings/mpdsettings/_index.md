---
title: "MpdSettings.MpdSettings"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor de MpdSettings. Inicializa una nueva instancia de la clase MpdSettings"
type: docs
weight: 10
url: /es/net/aspose.tasks.connectivity/mpdsettings/mpdsettings/
---
## MpdSettings constructor

Inicializa una nueva instancia de la clase [`MpdSettings`](../).

```csharp
public MpdSettings(string connectionString, int projectId)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| connectionString | Cadena | la cadena de conexión especificada. |
| projectId | Int32 | el id especificado de un proyecto para leer. |

## Ejemplos

Muestra cómo leer un proyecto desde un archivo MPD.

```csharp
DbSettings settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Ver también

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


