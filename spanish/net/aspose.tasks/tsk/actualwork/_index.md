---
title: "Tsk.ActualWork"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La cantidad de trabajo que ya ha sido realizado por los recursos asignados a las tareas"
type: docs
weight: 90
url: /es/net/aspose.tasks/tsk/actualwork/
---
## Tsk.ActualWork field

La cantidad de trabajo que ya ha sido realizado por los recursos asignados a tareas.

```csharp
public static readonly Key<Duration, TaskKey> ActualWork;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.ActualWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + task.Get(Tsk.ActualWork));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


