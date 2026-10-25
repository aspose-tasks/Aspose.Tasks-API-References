---
title: "Tsk.ActualFinish"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La fecha en que se completó una tarea"
type: docs
weight: 40
url: /es/net/aspose.tasks/tsk/actualfinish/
---
## Tsk.ActualFinish field

La fecha en que una tarea se completó.

```csharp
public static readonly Key<DateTime, TaskKey> ActualFinish;
```

## Ejemplos

Muestra que las fechas del proyecto se restablecen en modo de evaluación.

```csharp
var project = new Project();

// crear nuevas tareas
var task1 = project.RootTask.Children.Add("Task1");
task1.Set(Tsk.ActualStart, new DateTime(2000, 2, 10, 8, 0, 0));
task1.Set(Tsk.ActualFinish, new DateTime(2000, 2, 10, 17, 0, 0));

var task2 = project.RootTask.Children.Add("Task2");
task2.Set(Tsk.ActualStart, new DateTime(2000, 2, 10, 8, 0, 0));
task2.Set(Tsk.ActualFinish, new DateTime(2000, 2, 10, 17, 0, 0));

project.Save(OutDir + "EvaluationDateTimeLimitations_out.xml", SaveFileFormat.Xml);
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


