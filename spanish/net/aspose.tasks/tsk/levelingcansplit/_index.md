---
title: "Tsk.LevelingCanSplit"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Determina si la función de nivelación de recursos puede causar divisiones en el trabajo restante de esta tarea"
type: docs
weight: 760
url: /es/net/aspose.tasks/tsk/levelingcansplit/
---
## Tsk.LevelingCanSplit field

Determina si la función de nivelación de recursos puede causar divisiones en el trabajo restante de esta tarea.

```csharp
public static readonly Key<NullableBool, TaskKey> LevelingCanSplit;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.LevelingCanSplit.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingCanSplit, true);

Console.WriteLine("Leveling Can Split: " + task.Get(Tsk.LevelingCanSplit));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


