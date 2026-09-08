---
title: "Asn.ResponsePending"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. Determina si se ha recibido la respuesta para un mensaje TeamAssign"
type: docs
weight: 480
url: /es/net/aspose.tasks/asn/responsepending/
---
## Asn.ResponsePending field

Determina si se ha recibido la respuesta para un mensaje TeamAssign.

```csharp
public static readonly Key<bool, AsnKey> ResponsePending;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Asn.ResponsePending.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.ResponsePending, true);

Console.WriteLine("Response Pending: " + assignment.Get(Asn.ResponsePending));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


