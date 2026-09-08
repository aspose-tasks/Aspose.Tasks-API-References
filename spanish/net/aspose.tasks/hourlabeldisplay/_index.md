---
title: "Enumeración HourLabelDisplay"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.HourLabelDisplay. Especifica cómo se muestra la etiqueta de hora."
type: docs
weight: 820
url: /es/net/aspose.tasks/hourlabeldisplay/
---
## HourLabelDisplay enumeration

Especifica cómo se muestra la etiqueta de la hora.

```csharp
public enum HourLabelDisplay
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| H | `0` | "h" etiqueta. |
| Hr | `1` | "hr" etiqueta. |
| Hour | `2` | "hour(s)" etiqueta. |

## Ejemplos

Muestra cómo establecer la etiqueta de hora de las opciones de visualización del proyecto (caso 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// establece cómo se muestra la etiqueta de hora
project.DisplayOptions.HourLabel = HourLabelDisplay.H;

// ...
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


