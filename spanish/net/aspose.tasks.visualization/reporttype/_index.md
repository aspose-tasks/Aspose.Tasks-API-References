---
title: "Enumeración ReportType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.Visualization.ReportType enum. Tipo del informe gráfico de los proyectos"
type: docs
weight: 3330
url: /es/net/aspose.tasks.visualization/reporttype/
---
## ReportType enumeration

Tipo del informe gráfico del proyecto.

```csharp
public enum ReportType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| ProjectOverview | `0` | Muestra la fecha de inicio y fin del proyecto, el porcentaje de duración completado, el porcentaje completado de las tareas de nivel superior y los hitos próximos. |
| CostOverview | `1` | Muestra las fechas de inicio y fin del proyecto, el costo programado y restante actual, % completado y los valores de costo para las tareas de nivel superior. |
| WorkOverview | `2` | Muestra la línea base, el trabajo real y el trabajo restante para cada tarea de nivel superior y el trabajo para los recursos de trabajo. |
| ResourceOverview | `3` | Muestra la línea base, el trabajo real y el trabajo restante por recurso. |
| ResourceCostOverview | `4` | Muestra la línea base, el costo real y el costo restante por recurso. |
| CriticalTasks | `5` | Muestra las tareas del proyecto que son críticas. |
| LateTasks | `6` | Muestra las tareas del proyecto que están retrasadas. |
| Milestones | `7` | Muestra los hitos que están retrasados, próximos y completados. |
| UpcomingTask | `8` | Muestra las tareas que vencen durante la semana actual y las tareas que comienzan durante la semana actual. |
| CostOverruns | `9` | Muestra la variación de costos por tarea y recurso. |
| TaskCostOverview | `10` | Muestra la línea base, el costo real y el costo restante de todas las tareas de nivel superior. |
| OverallocatedResources | `11` | Muestra el número de horas de trabajo restantes para recursos sobreasignados. |
| SlippingTasks | `12` | Muestra las tareas que deben finalizar después de sus fechas de fin de línea base (la línea base debe estar establecida). |
| BestPracticeAnalyzer | `13` | Muestra tareas sin trabajo real, tareas no asignadas, tareas con duración inferior a 8 horas y resúmenes asignados con los recursos. |
| Burndown | `14` | Incluye gráficos de agotamiento de trabajo y de agotamiento de tareas. El gráfico de agotamiento de trabajo muestra cuánto trabajo han terminado las personas, cuánto está programado para terminar antes de la fecha de finalización del proyecto, y la estimación de línea base de cuánto trabajo se completaría en este punto del proyecto. El gráfico de agotamiento de tareas muestra el número de tareas terminadas, el número restante y la estimación de línea base de cuántas se terminarían en este punto del proyecto. |
| CashFlow | `15` | Muestra los costos y los costos acumulados por trimestre para todas las tareas de nivel superior. |

## Ejemplos

Muestra cómo guardar el informe de disminución del proyecto en formato PDF en el flujo especificado.

```csharp
var project = new Project(DataDir + @"Homemoveplan.mpp");
using (var stream = new FileStream(OutDir + "Burndown_out.pdf", FileMode.Create))
{
    project.SaveReport(stream, ReportType.Burndown);
}
```

### Ver también

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


