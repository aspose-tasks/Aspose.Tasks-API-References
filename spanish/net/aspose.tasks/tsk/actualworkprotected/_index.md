---
title: "Tsk.ActualWorkProtected"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La duración durante la cual el trabajo real está protegido. Lectura compatible solo con formato XML."
type: docs
weight: 100
url: /es/net/aspose.tasks/tsk/actualworkprotected/
---
## Tsk.ActualWorkProtected field

La duración durante la cual el trabajo real está protegido. Lectura compatible solo con formato XML.

```csharp
public static readonly Key<Duration, TaskKey> ActualWorkProtected;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.ActualWorkProtected.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + task.Get(Tsk.ActualWorkProtected));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


