---
title: "Enum MonthLabelDisplay"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.MonthLabelDisplay enum. Especifica cómo se muestra la etiqueta del mes"
type: docs
weight: 1060
url: /es/net/aspose.tasks/monthlabeldisplay/
---
## MonthLabelDisplay enumeration

Especifica cómo se muestra la etiqueta del mes.

```csharp
public enum MonthLabelDisplay
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Mo | `0` | Establece la lista de meses en MS Project como mo. |
| Mon | `1` | Establece la lista de meses en MS Project como mon. |
| Month | `2` | Establece la lista de meses en MS Project como month. |

## Ejemplos

Muestra cómo establecer la etiqueta del mes en las opciones de visualización del proyecto (caso 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// establecer cómo se muestra la etiqueta del mes
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mo;

// ...
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


