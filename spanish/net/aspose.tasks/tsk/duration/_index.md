---
title: "Tsk.Duration"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. El período total de tiempo de trabajo activo para una tarea, según se ingrese o según lo calcule Microsoft Project basándose en la fecha de inicio, fecha de fin, calendarios y otros factores de programación."
type: docs
weight: 300
url: /es/net/aspose.tasks/tsk/duration/
---
## Tsk.Duration field

El período total de tiempo de trabajo activo para una tarea según se ingresó o según lo calcule Microsoft Project basándose en la fecha de inicio, fecha de finalización, calendarios y otros factores de programación.

```csharp
public static readonly Key<Duration, TaskKey> Duration;
```

## Ejemplos

Muestra cómo establecer la duración de la tarea.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddTaskDuration_out.xml", SaveFileFormat.Xml);
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


