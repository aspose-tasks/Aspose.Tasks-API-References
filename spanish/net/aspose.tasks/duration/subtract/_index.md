---
title: "Duration.Subtract"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Duration. Resta la duración especificada de esta instancia de duración."
type: docs
weight: 100
url: /es/net/aspose.tasks/duration/subtract/
---
## Subtract(Duration) {#subtract}

Resta la duración especificada de esta instancia de duración.

```csharp
public Duration Subtract(Duration d)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| d | Duration | la instancia especificada de [`Duration`](../) para restar de esta instancia. |

### Valor devuelto

Nuevo objeto de duración que representa el valor de esta instancia menos el valor de duración especificado.

## Ejemplos

Muestra cómo cambiar la duración de las tareas.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// obtener una tarea
var task1 = project.RootTask.Children.GetById(1);

// actualizar la duración de la tarea
var duration1 = task1.Get(Tsk.Duration);

// restar un día a la tarea 1
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// establecer una nueva duración a la tarea
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// obtener otra tarea
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// cambiar la duración usando el tipo de unidad de tiempo actual
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// establecer una nueva duración a la tarea
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### Ver también

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)

---

## Subtract(double) {#subtract_1}

Resta el valor double especificado de esta instancia de duración.

```csharp
public Duration Subtract(double val)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | Double | valor Double especificado para restar de esta instancia. |

### Valor devuelto

Nuevo objeto de duración que representa el valor de esta instancia menos el valor de duración especificado.

## Ejemplos

Muestra cómo cambiar la duración de las tareas.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// obtener una tarea
var task1 = project.RootTask.Children.GetById(1);

// actualizar la duración de la tarea
var duration1 = task1.Get(Tsk.Duration);

// restar un día a la tarea 1
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// establecer una nueva duración a la tarea
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// obtener otra tarea
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// cambiar la duración usando el tipo de unidad de tiempo actual
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// establecer una nueva duración a la tarea
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### Ver también

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


