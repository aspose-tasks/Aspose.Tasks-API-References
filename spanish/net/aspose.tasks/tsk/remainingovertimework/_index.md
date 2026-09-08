---
title: "Tsk.RemainingOvertimeWork"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La cantidad de tiempo extra programado restante."
type: docs
weight: 980
url: /es/net/aspose.tasks/tsk/remainingovertimework/
---
## Tsk.RemainingOvertimeWork field

La cantidad de tiempo restante programado de horas extra.

```csharp
public static readonly Key<Duration, TaskKey> RemainingOvertimeWork;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.RemainingOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + task.Get(Tsk.RemainingOvertimeWork));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


