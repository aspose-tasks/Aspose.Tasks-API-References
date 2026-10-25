---
title: "Project.Recalculate"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método de Project. Reprograma todas las tareas del proyecto, sus IDs, niveles de esquema, fechas de inicio/fin, establece fechas tempranas/tardías, calcula holguras, trabajo y campos de costo."
type: docs
weight: 1150
url: /es/net/aspose.tasks/project/recalculate/
---
## Recalculate() {#recalculate}

Reprograma los IDs de todas las tareas del proyecto, los niveles de esquema, las fechas de inicio/fin, establece las fechas tempranas/tardías, calcula holguras, trabajo y campos de costo.

```csharp
public void Recalculate()
```

## Ejemplos

Muestra cómo reprogramar el proyecto a partir de la fecha de inicio en lugar de la fecha de finalización.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, new DateTime(2014, 1, 1));

// Ahora se calculan todas las fechas de las tareas (Start, Finish, EarlyStart, EarlyFinish, LateStart, LateFinish). Para obtener la ruta crítica necesitamos calcular los holguras (puede invocarse en un hilo separado, pero solo después del cálculo de todas las fechas tempranas/tardías).
project.Recalculate();

foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id));
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### Ver también

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Recalculate(bool) {#recalculate_1}

Reprograma los IDs de todas las tareas del proyecto, los niveles de esquema, las fechas de inicio/fin, establece las fechas tempranas/tardías, calcula holguras, trabajo y campos de costo con validación opcional.

```csharp
public void Recalculate(bool validate)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| validate | Boolean | Si es verdadero, se realizará la validación de recalculación. Qué datos se validan: Por el momento solo se implementa la validación básica de los rangos de fechas de tareas y enlaces de tareas. Los rangos de fechas de las tareas (p. ej., ActualStart - ActualFinish, EarlyStart - EarlyFinish, etc.) así como las fechas de los enlaces de tareas se comprobarán contra el criterio de que la fecha de inicio sea menor o igual que la fecha de finalización. Si alguna de las condiciones descritas arriba falla, se lanzará [`RecalculationValidationException`](../../recalculationvalidationexception/). |

## Ejemplos

Muestra cómo recalcular el proyecto con validación posterior.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("t1");
task.Set(Tsk.CommitmentStart, new DateTime(2017, 6, 19, 8, 0, 0));
task.Set(Tsk.CommitmentFinish, new DateTime(2017, 6, 18, 17, 0, 0));

try
{
    // recalcular el proyecto con validación posterior
    project.Recalculate(true);
}
catch (TaskValidationException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Ver también

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


