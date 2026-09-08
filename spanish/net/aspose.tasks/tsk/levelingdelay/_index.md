---
title: "Tsk.LevelingDelay"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. El tiempo que una tarea debe retrasarse desde su fecha de inicio temprana debido al nivelado de recursos"
type: docs
weight: 770
url: /es/net/aspose.tasks/tsk/levelingdelay/
---
## Tsk.LevelingDelay field

El tiempo que una tarea debe retrasarse desde su fecha de inicio temprana debido a la nivelación de recursos.

```csharp
public static readonly Key<Duration, TaskKey> LevelingDelay;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.LevelingDelay.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingDelay, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Leveling Delay: " + task.Get(Tsk.LevelingDelay));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


