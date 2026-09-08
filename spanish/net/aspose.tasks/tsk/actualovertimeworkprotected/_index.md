---
title: "Tsk.ActualOvertimeWorkProtected"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La duración durante la cual el trabajo real de horas extra está protegido"
type: docs
weight: 70
url: /es/net/aspose.tasks/tsk/actualovertimeworkprotected/
---
## Tsk.ActualOvertimeWorkProtected field

La duración durante la cual el trabajo extra real está protegido.

```csharp
public static readonly Key<Duration, TaskKey> ActualOvertimeWorkProtected;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.ActualOvertimeWorkProtected.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Overtime Work Protected: " + task.Get(Tsk.ActualOvertimeWorkProtected));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


