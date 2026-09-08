---
title: "Project.GetBaselineSaveTime"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Project. Devuelve la hora de guardado de la línea base"
type: docs
weight: 1090
url: /es/net/aspose.tasks/project/getbaselinesavetime/
---
## Project.GetBaselineSaveTime method

Devuelve la hora de guardado de la línea base.

```csharp
public DateTime GetBaselineSaveTime(BaselineType baselineNumber)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| baselineNumber | BaselineType | El número de la línea base [`BaselineType`](../../baselinetype/). |

### Valor devuelto

La última fecha y hora de guardado de la línea base.

## Observaciones

Devuelve DateTime.MinValue si la línea base no se guardó.

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


