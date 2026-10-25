---
title: "Tsk.ActualOvertimeWork"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La cantidad real de trabajo extra ya realizado por los recursos asignados a las tareas"
type: docs
weight: 60
url: /es/net/aspose.tasks/tsk/actualovertimework/
---
## Tsk.ActualOvertimeWork field

La cantidad real de trabajo extra ya realizado por los recursos asignados a tareas.

```csharp
public static readonly Key<Duration, TaskKey> ActualOvertimeWork;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.ActualOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + task.Get(Tsk.ActualOvertimeWork));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


