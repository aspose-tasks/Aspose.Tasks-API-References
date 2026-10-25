---
title: "Tsk.ActivityId"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Representa el campo de ID de actividad, un identificador único de tarea utilizado por Primavera. Solo aplicable a proyectos Primavera"
type: docs
weight: 10
url: /es/net/aspose.tasks/tsk/activityid/
---
## Tsk.ActivityId field

Representa el campo id de actividad - el identificador único de una tarea utilizado por Primavera. (solo aplicable a proyectos Primavera).

```csharp
public static readonly Key<string, TaskKey> ActivityId;
```

## Ejemplos

Muestra cómo trabajar con el campo ActivityId específico de proyectos Primavera

```csharp
var project = new Project(DataDir + "test.xer");

var task = project.RootTask.Children.GetById(1);

Console.WriteLine("Task activity_id: {0}", task.Get(Tsk.ActivityId));

task.Set(Tsk.ActivityId, "CUSTOM_ACTIVITY_ID");

// Cree opciones de guardado de Primavera y especifique que los ActivityIds no deben sobrescribirse durante el guardado.
var options = new PrimaveraSaveOptions
{
    RenumberActivityIds = false
};

project.Save(OutDir + "WorkWithPrimaveraActivityId_out.xer", options);
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


