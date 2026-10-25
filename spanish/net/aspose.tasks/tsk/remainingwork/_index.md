---
title: "Tsk.RemainingWork"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. El tiempo aún necesario para completar una tarea o un conjunto de tareas."
type: docs
weight: 990
url: /es/net/aspose.tasks/tsk/remainingwork/
---
## Tsk.RemainingWork field

El tiempo aún necesario para completar una tarea o conjunto de tareas.

```csharp
public static readonly Key<Duration, TaskKey> RemainingWork;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.RemainingWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + task.Get(Tsk.RemainingWork));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


