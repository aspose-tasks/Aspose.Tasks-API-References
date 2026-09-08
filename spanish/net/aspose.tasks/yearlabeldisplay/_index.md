---
title: "Enumeración YearLabelDisplay"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.YearLabelDisplay. Especifica cómo se muestra la etiqueta del año"
type: docs
weight: 3680
url: /es/net/aspose.tasks/yearlabeldisplay/
---
## YearLabelDisplay enumeration

Especifica cómo se muestra la etiqueta del año.

```csharp
public enum YearLabelDisplay
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Y | `0` | Establece la lista de años en MS Project como mo. |
| Yr | `1` | Establece la lista de años en MS Project como mon. |
| Year | `2` | Establece la lista de Años en MS Project como mes. |

## Ejemplos

Muestra cómo establecer la etiqueta del año de las opciones de visualización del proyecto (caso 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// establece cómo se muestra la etiqueta del año
project.DisplayOptions.YearLabel = YearLabelDisplay.Y;

// ...
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


