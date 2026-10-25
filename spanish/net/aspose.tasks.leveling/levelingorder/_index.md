---
title: "Enum LevelingOrder"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enum Aspose.Tasks.Leveling.LevelingOrder. Define los valores posibles del orden de nivelado"
type: docs
weight: 950
url: /es/net/aspose.tasks.leveling/levelingorder/
---
## LevelingOrder enumeration

Define los valores posibles del orden de nivelado.

```csharp
public enum LevelingOrder
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Standard | `1` | Se tienen en cuenta las siguientes propiedades: relaciones de predecesores, holgura total (una tarea con mayor holgura total se retrasa primero), fecha de inicio, prioridad. Este es el valor predeterminado. |
| IdOnly | `2` | Las tareas se retrasan en orden ascendente de Id. |
| PriorityThenStandard | `3` | Se considera primero la prioridad, luego las mismas propiedades que en Standard. |

### Ver también

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


