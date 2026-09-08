---
title: "Enum DayLabelDisplay"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.DayLabelDisplay enum. Especifica cómo se muestra la etiqueta del día"
type: docs
weight: 440
url: /es/net/aspose.tasks/daylabeldisplay/
---
## DayLabelDisplay enumeration

Especifica cómo se muestra la etiqueta del día.

```csharp
public enum DayLabelDisplay
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| D | `0` | Establece la lista de Días en MS Project como d. |
| Dy | `1` | Establece la lista de Días en MS Project como dy. |
| Day | `2` | Establece la lista de Días en MS Project como day. |

## Ejemplos

Muestra cómo establecer la etiqueta de día de las opciones de visualización del proyecto (caso 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// establece cómo se muestra la etiqueta del día
project.DisplayOptions.DayLabel = DayLabelDisplay.D;

// ...
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


