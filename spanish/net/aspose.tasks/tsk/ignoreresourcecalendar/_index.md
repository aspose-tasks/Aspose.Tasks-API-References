---
title: "Tsk.IgnoreResourceCalendar"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Determina si la programación de la tarea considera los calendarios de los recursos asignados a la tarea"
type: docs
weight: 530
url: /es/net/aspose.tasks/tsk/ignoreresourcecalendar/
---
## Tsk.IgnoreResourceCalendar field

Determina si la programación de la tarea considera los calendarios de los recursos asignados a la tarea.

```csharp
public static readonly Key<NullableBool, TaskKey> IgnoreResourceCalendar;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.IgnoreResourceCalendar.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IgnoreResourceCalendar, true);

Console.WriteLine("Ignore Resource Calendar: " + task.Get(Tsk.IgnoreResourceCalendar));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


