---
title: "Enum WeekLabelDisplay"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.WeekLabelDisplay enum. Especifica cómo se muestra la etiqueta de la semana"
type: docs
weight: 3560
url: /es/net/aspose.tasks/weeklabeldisplay/
---
## WeekLabelDisplay enumeration

Especifica cómo se muestra la etiqueta de la semana.

```csharp
public enum WeekLabelDisplay
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| W | `0` | "w" etiqueta. |
| Wk | `1` | "wk" etiqueta. |
| Week | `2` | "week" etiqueta. |

## Ejemplos

Muestra cómo establecer la etiqueta de semana de las opciones de visualización del proyecto (caso 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// establece cómo se muestra la etiqueta de la semana
project.DisplayOptions.WeekLabel = WeekLabelDisplay.W;

// ...
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


