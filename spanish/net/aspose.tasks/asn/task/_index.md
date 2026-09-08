---
title: "Asn.Task"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. La tarea a la que se asigna un recurso"
type: docs
weight: 550
url: /es/net/aspose.tasks/asn/task/
---
## Asn.Task field

La tarea a la que se asigna un recurso.

```csharp
public static readonly Key<Task, AsnKey> Task;
```

## Ejemplos

Muestra cómo leer las propiedades Asn.Task y Asn.Resource.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Assigned Task Name: " + assignment.Get(Asn.Task).Get(Tsk.Name));
Console.WriteLine("Assigned Resource Name: " + assignment.Get(Asn.Resource).Get(Rsc.Name));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Task](../../task/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


