---
title: "Tsk.Work"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. El tiempo total programado en una tarea para todos los recursos asignados"
type: docs
weight: 1150
url: /es/net/aspose.tasks/tsk/work/
---
## Tsk.Work field

El tiempo total programado en una tarea para todos los recursos asignados.

```csharp
public static readonly Key<Duration, TaskKey> Work;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.Work.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Work, project.GetWork(1));

Console.WriteLine("Work: " + task.Get(Tsk.Work));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


