---
title: "Tsk.LevelAssignments"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Determina si la función de nivelación puede retrasar y dividir asignaciones individuales para resolver sobreasignaciones"
type: docs
weight: 750
url: /es/net/aspose.tasks/tsk/levelassignments/
---
## Tsk.LevelAssignments field

Determina si la función de nivelación puede retrasar y dividir asignaciones individuales para resolver sobreasignaciones.

```csharp
public static readonly Key<NullableBool, TaskKey> LevelAssignments;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.LevelAssignments.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelAssignments, true);

Console.WriteLine("Level Assignments: " + task.Get(Tsk.LevelAssignments));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


