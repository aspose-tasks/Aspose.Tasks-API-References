---
title: "Asn.Confirmed"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. Determina si un recurso ha aceptado todas sus asignaciones"
type: docs
weight: 170
url: /es/net/aspose.tasks/asn/confirmed/
---
## Asn.Confirmed field

Determina si un recurso ha aceptado todas sus asignaciones.

```csharp
public static readonly Key<bool, AsnKey> Confirmed;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Asn.Confirmed.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Confirmed, true);

Console.WriteLine("Confirmed: " + assignment.Get(Asn.Confirmed));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


