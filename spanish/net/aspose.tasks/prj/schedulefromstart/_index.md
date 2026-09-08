---
title: "Prj.ScheduleFromStart"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. Determina si se debe calcular el cronograma del proyecto hacia adelante desde la fecha de inicio"
type: docs
weight: 630
url: /es/net/aspose.tasks/prj/schedulefromstart/
---
## Prj.ScheduleFromStart field

Determina si se debe calcular el cronograma del proyecto hacia adelante desde la fecha de inicio.

```csharp
public static readonly Key<NullableBool, PrjKey> ScheduleFromStart;
```

## Ejemplos

Muestra cómo reprogramar el proyecto a partir de la fecha de finalización en lugar de la de inicio.

```csharp
var project = new Project();
project.Set(Prj.ScheduleFromStart, false);
project.Set(Prj.FinishDate, new DateTime(2020, 1, 1));

// Ahora se calculan todas las fechas de las tareas (Start, Finish, EarlyStart, EarlyFinish, LateStart, LateFinish). Para obtener la ruta crítica necesitamos calcular los holguras (puede invocarse en un hilo separado, pero solo después del cálculo de todas las fechas tempranas/tardías).
project.Recalculate();

foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id));
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


