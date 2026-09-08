---
title: "Tsk.RegularWork"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La cantidad total de trabajo sin horas extra programado para ser realizado por los recursos"
type: docs
weight: 940
url: /es/net/aspose.tasks/tsk/regularwork/
---
## Tsk.RegularWork field

La cantidad total de trabajo no extra programado para ser realizado por los recursos.

```csharp
public static readonly Key<Duration, TaskKey> RegularWork;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.RegularWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + task.Get(Tsk.RegularWork));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


