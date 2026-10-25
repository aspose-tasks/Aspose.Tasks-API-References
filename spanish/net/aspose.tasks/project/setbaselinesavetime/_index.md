---
title: "Project.SetBaselineSaveTime"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método de Project. Establece la hora de guardado de la línea base."
type: docs
weight: 1260
url: /es/net/aspose.tasks/project/setbaselinesavetime/
---
## Project.SetBaselineSaveTime method

Establece la hora de guardado de la línea base.

```csharp
public void SetBaselineSaveTime(BaselineType baselineNumber, DateTime value)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| baselineNumber | BaselineType | El número de la línea base [`BaselineType`](../../baselinetype/). |
| value | DateTime | La última fecha y hora de guardado de la línea base. |

## Observaciones

Establezca el valor a DateTime.MinValue si la línea base no se guardó.

## Ejemplos

Muestra cómo leer/escribir el tiempo de guardado de la línea base del proyecto.

```csharp
var project = new Project();
var baselineSave = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time before: " + baselineSave);

// establecer tiempo de guardado de la línea base
project.SetBaselineSaveTime(BaselineType.Baseline, DateTime.Today);

var baselineSaveNew = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time after: " + baselineSaveNew);
```

### Ver también

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


