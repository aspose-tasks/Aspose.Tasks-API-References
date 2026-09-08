---
title: "Tsk.Stop"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La fecha que representa el final de la parte real de una tarea"
type: docs
weight: 1060
url: /es/net/aspose.tasks/tsk/stop/
---
## Tsk.Stop field

La fecha que representa el final de la parte real de una tarea.

```csharp
public static readonly Key<DateTime, TaskKey> Stop;
```

## Ejemplos

Muestra cómo leer las fechas de Detener/Reanudar de la tarea.

```csharp
var project = new Project(DataDir + "StopResumeDates.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Verificar las fechas de Detener y Reanudar para todas las tareas
foreach (var task in collector.Tasks)
{
    if (task.Get(Tsk.Stop).ToShortDateString() == "1/1/2000")
    {
        Console.WriteLine("Stop: NA");
    }
    else
    {
        Console.WriteLine("Stop: " + task.Get(Tsk.Stop).ToShortDateString());
    }

    if (task.Get(Tsk.Resume).ToShortDateString() == "1/1/2000")
    {
        Console.WriteLine("Resume: NA");
    }
    else
    {
        Console.WriteLine("Resume: " + task.Get(Tsk.Resume).ToShortDateString());
    }
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


