---
title: "Enum GroupOn"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.GroupOn enum. Especifica el tipo de agrupación"
type: docs
weight: 810
url: /es/net/aspose.tasks/groupon/
---
## GroupOn enumeration

Especifica el tipo de agrupación.

```csharp
public enum GroupOn
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| DateDay | `13` | Agrupar por fecha por día. |
| DateEachValue | `10` | Agrupar por fecha para cada valor. |
| DateHour | `12` | Agrupar por fecha por hora. |
| DateMinute | `11` | Agrupar por fecha por minuto. |
| DateMonth | `16` | Agrupar por fecha por mes. |
| DateQtr | `17` | Agrupar por fecha por trimestre. |
| DateThirdOfMonth | `15` | Agrupar por fecha por cada tercio de un mes. |
| DateWeek | `14` | Agrupar por fecha por semana. |
| DateYear | `18` | Agrupar por fecha por año. |
| DurationDays | `23` | Agrupar por duración por días. |
| DurationEachValue | `20` | Agrupar por duración para cada valor. |
| DurationHours | `22` | Agrupar por duración por horas. |
| DurationMinutes | `21` | Agrupar por duración por minutos. |
| DurationMonths | `25` | Agrupar por duración por meses. |
| DurationWeeks | `24` | Agrupar por duración por semanas. |
| EachValue | `0` | Agrupar por cada valor. |
| Interval | `1` | Agrupar por el intervalo. |
| OutlineEachValue | `30` | Agrupar por cada valor de contorno. |
| OutlineLevel | `31` | Agrupar por el nivel de contorno. |
| Pct110 | `45` | Agrupar por incrementos de finalización del 10 por ciento. |
| Pct125 | `44` | Agrupar por incrementos de finalización del 25 por ciento. |
| Pct150 | `43` | Agrupar por incrementos de finalización del 50 por ciento. |
| Pct199 | `42` | Agrupar por finalización del 99 por ciento. |
| PctEachValue | `40` | Agrupar por porcentaje de cada valor. |
| PctInterval | `41` | Agrupar por el porcentaje del intervalo. |
| TextEachValue | `50` | Agrupar por cada valor de texto. |
| TextPrefix | `51` | Agrupar por el prefijo de texto. |

## Ejemplos

Muestra cómo leer las propiedades de un criterio de grupo.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

Console.WriteLine("Task Groups Count: " + project.TaskGroups.Count);
var group = project.TaskGroups.ToList()[1];
Console.WriteLine("Task Group Name: " + group.Name);
Console.WriteLine("Task Group Criteria count: " + group.GroupCriteria.Count);

Console.WriteLine("\n************* Retrieving Task Group's Criterion information *************");
var criterion = group.GroupCriteria.ToList()[0];
Console.WriteLine("Task Criterion Field: " + criterion.Field);
Console.WriteLine("Task Criterion GroupOn: " + criterion.GroupOn);
Console.WriteLine("Task Criterion Cell Color: " + criterion.CellColor);
Console.WriteLine("Task Criterion Font Color: " + criterion.FontColor);
Console.WriteLine("Task Criterion Group Interval: " + criterion.GroupInterval);
Console.WriteLine("Task Criterion Start At: " + criterion.StartAt);

// Lee el patrón de fondo del criterio.
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


