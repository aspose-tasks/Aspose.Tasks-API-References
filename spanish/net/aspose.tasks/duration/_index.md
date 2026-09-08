---
title: "Estructura Duration"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Estructura Aspose.Tasks.Duration. Representa la duración en un proyecto."
type: docs
weight: 470
url: /es/net/aspose.tasks/duration/
---
## Duration structure

Representa la duración en un proyecto.

```csharp
public struct Duration : IEquatable<Duration>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [IsElapsed](../../aspose.tasks/duration/iselapsed/) { get; } | Obtiene un valor que indica si la unidad de tiempo está transcurrida. La bandera que determina si esta instancia de Duration está transcurrida. |
| [IsEstimated](../../aspose.tasks/duration/isestimated/) { get; } | Obtiene un valor que indica si la unidad de tiempo está estimada. La bandera que determina si esta instancia de Duration está estimada. |
| [TimeSpan](../../aspose.tasks/duration/timespan/) { get; } | Obtiene la instancia [`TimeSpan`](./timespan/) de este objeto Duration. La instancia TimeSpan de este objeto Duration. |
| [TimeUnit](../../aspose.tasks/duration/timeunit/) { get; } | Obtiene el tipo de unidad de tiempo para este objeto. El tipo de unidad de tiempo de esta instancia Duration. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [Parse](../../aspose.tasks/duration/parse/)(Project, string) | Convierte la cadena especificada a la instancia de la estructura `Duration`. |
| [Add](../../aspose.tasks/duration/add/#add_1)(double) | Agrega el valor double especificado a esta duración. |
| [Add](../../aspose.tasks/duration/add/#add)(Duration) | Agrega la duración especificada a esta duración. |
| [Convert](../../aspose.tasks/duration/convert/)(TimeUnitType) | Convierte el objeto Duration a otra duración con unidades de tiempo especificadas. |
| [Equals](../../aspose.tasks/duration/equals/#equals)(Duration) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| override [Equals](../../aspose.tasks/duration/equals/#equals_1)(object) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| override [GetHashCode](../../aspose.tasks/duration/gethashcode/)() | Devuelve un valor de código hash para este objeto. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract_1)(double) | Resta el valor double especificado de esta instancia de duración. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract)(Duration) | Resta la duración especificada de esta instancia de duración. |
| [ToDouble](../../aspose.tasks/duration/todouble/)() | Convierte el objeto Duration a un valor Double. |
| override [ToString](../../aspose.tasks/duration/tostring/)() | Devuelve una representación en cadena de esta instancia. |
| static [ParseTimeSpan](../../aspose.tasks/duration/parsetimespan/)(string) | Analiza la cadena de duración en el formato "PT--H--M--S--". |
| [operator ==](../../aspose.tasks/duration/op_equality/) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [operator !=](../../aspose.tasks/duration/op_inequality/) | Devuelve un valor que indica si esta instancia no es igual a un objeto especificado. |

## Ejemplos

Muestra cómo actualizar una duración de tareas.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// obtener una tarea
var task1 = project.RootTask.Children.GetById(1);

// actualizar la duración de la tarea
var duration1 = task1.Get(Tsk.Duration);

// agregar un día a la tarea 1
duration1 = duration1.Add(project.GetDuration(1, TimeUnitType.Day));

// establecer una nueva duración a la tarea
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// obtener otra tarea
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// cambiar la duración usando el tipo de unidad de tiempo actual
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Add(1d /* the time unit type of duration2 will be used */);

// establecer una nueva duración a la tarea
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task1.Get(Tsk.Duration));
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


