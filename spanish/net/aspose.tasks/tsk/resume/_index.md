---
title: "Tsk.Resume"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La fecha en que la parte restante de una tarea está programada para reanudarse después de registrar cualquier progreso"
type: docs
weight: 1000
url: /es/net/aspose.tasks/tsk/resume/
---
## Tsk.Resume field

La fecha en que la parte restante de una tarea está programada para reanudarse después de iniciar cualquier progreso.

```csharp
public static readonly Key<DateTime, TaskKey> Resume;
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


