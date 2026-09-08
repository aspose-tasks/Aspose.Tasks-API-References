---
title: "Enumeración MinuteLabelDisplay"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.MinuteLabelDisplay. Especifica cómo se muestra la etiqueta de minuto."
type: docs
weight: 1030
url: /es/net/aspose.tasks/minutelabeldisplay/
---
## MinuteLabelDisplay enumeration

Especifica cómo se muestra la etiqueta de los minutos.

```csharp
public enum MinuteLabelDisplay
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| M | `0` | Establece la lista Minutes en MS Project como m. |
| Min | `1` | Establece la lista Minutes en MS Project como min. |
| Minute | `2` | Establece la lista Minutes en MS Project como minute. |

## Ejemplos

Muestra cómo establecer la etiqueta de minuto de las opciones de visualización del proyecto (caso 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// establece cómo se muestra la etiqueta de minuto
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.M;

// ...
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


