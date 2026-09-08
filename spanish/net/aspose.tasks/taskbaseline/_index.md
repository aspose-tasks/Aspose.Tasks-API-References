---
title: "Clase TaskBaseline"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.TaskBaseline. Representa la línea base de una tarea"
type: docs
weight: 2370
url: /es/net/aspose.tasks/taskbaseline/
---
## TaskBaseline class

Representa la línea base de una tarea.

```csharp
public sealed class TaskBaseline : Baseline, IComparable<TaskBaseline>, IEquatable<TaskBaseline>
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [TaskBaseline](taskbaseline/)(Task) | Inicializa una nueva instancia de la clase `TaskBaseline`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | Obtiene o establece el número único de un registro de datos de línea base. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | Obtiene o establece el costo presupuestado del trabajo realizado por un recurso para un proyecto hasta la fecha. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | Obtiene o establece el costo presupuestado de un trabajo programado para un recurso. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | Obtiene o establece el costo proyectado de un recurso cuando se guarda la línea base. |
| [Duration](../../aspose.tasks/taskbaseline/duration/) { get; set; } | Obtiene o establece la duración programada de la tarea cuando se guardó la línea base. |
| [EstimatedDuration](../../aspose.tasks/taskbaseline/estimatedduration/) { get; set; } | Obtiene o establece un valor que indica si la duración de la línea base de la tarea fue estimada. |
| [Finish](../../aspose.tasks/taskbaseline/finish/) { get; set; } | Obtiene o establece la fecha de finalización programada de la tarea cuando se guardó la línea base. |
| [FixedCost](../../aspose.tasks/taskbaseline/fixedcost/) { get; set; } | Obtiene o establece un costo fijo de la tarea cuando se guardó la línea base. |
| [Interim](../../aspose.tasks/taskbaseline/interim/) { get; set; } | Obtiene o establece un valor que indica si esta es una Línea Base Intermedia. |
| [Start](../../aspose.tasks/taskbaseline/start/) { get; set; } | Obtiene o establece la fecha de inicio programada de la tarea cuando se guardó la línea base. |
| [TimephasedData](../../aspose.tasks/taskbaseline/timephaseddata/) { get; set; } | Obtiene o establece una instancia de TimephasedDataCollection para este objeto. Los datos temporales asociados con la línea base de la tarea. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | Obtiene o establece el trabajo asignado a un recurso cuando se guarda la línea base. La cantidad de trabajo asignado a un recurso cuando se guardó la línea base. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | Implementación de la interfaz IComparable. Compara esta instancia con el objeto Baseline especificado. |
| [CompareTo](../../aspose.tasks/taskbaseline/compareto/#compareto_1)(TaskBaseline) | Implementación de la interfaz IComparable. Compara esta instancia con el objeto Baseline especificado. |
| [Equals](../../aspose.tasks/baseline/equals/)(Baseline) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| override [Equals](../../aspose.tasks/taskbaseline/equals/#equals_2)(object) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [Equals](../../aspose.tasks/taskbaseline/equals/#equals_1)(TaskBaseline) | Devuelve un valor que indica si esta instancia es igual al objeto TaskBaseline especificado. |
| override [GetHashCode](../../aspose.tasks/taskbaseline/gethashcode/)() | Devuelve un valor de código hash para la instancia de la clase `TaskBaseline`. |

## Ejemplos

Muestra cómo obtener acceso a la información de la línea base.

```csharp
var project = new Project();

// Creando TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// Mostrar duración de la línea base de la tarea
var baseline = task.Baselines.ToList()[0];
Console.WriteLine("Baseline Start: {0}", baseline.Start);
Console.WriteLine("Baseline duration: {0}", baseline.Duration);
Console.WriteLine("Baseline duration format: {0}", baseline.Duration.TimeUnit);
Console.WriteLine("Is it estimated duration?: {0}", baseline.EstimatedDuration);
Console.WriteLine("Baseline Finish: {0}", baseline.Finish);

// valor que indica si esta es una Línea Base Intermedia
Console.WriteLine("Interim: {0}", baseline.Interim);
Console.WriteLine("Fixed Cost: {0}", baseline.FixedCost);

// imprimir datos temporales de la línea base de la tarea
Console.WriteLine("Number of timephased items: " + baseline.TimephasedData.Count);
foreach (var data in baseline.TimephasedData)
{
    Console.WriteLine(" Uid: " + data.Uid);
    Console.WriteLine(" Start: " + data.Start);
    Console.WriteLine(" Finish: " + data.Finish);
}
```

### Ver también

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


