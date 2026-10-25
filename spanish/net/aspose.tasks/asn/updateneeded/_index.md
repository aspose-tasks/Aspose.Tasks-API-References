---
title: "Asn.UpdateNeeded"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. Determina si el recurso asignado a una tarea necesita ser actualizado respecto al estado de la tarea"
type: docs
weight: 580
url: /es/net/aspose.tasks/asn/updateneeded/
---
## Asn.UpdateNeeded field

Determina si el recurso asignado a una tarea necesita actualizarse respecto al estado de la tarea.

```csharp
public static readonly Key<bool, AsnKey> UpdateNeeded;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Asn.UpdateNeeded.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.UpdateNeeded, true);

Console.WriteLine("Update Needed: " + assignment.Get(Asn.UpdateNeeded));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


