---
title: "Asn.Uid"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. El identificador único de una asignación"
type: docs
weight: 560
url: /es/net/aspose.tasks/asn/uid/
---
## Asn.Uid field

El identificador único de una asignación.

```csharp
public static readonly Key<int, AsnKey> Uid;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Asn.Uid.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Uid, 30);

Console.WriteLine("UID: " + assignment.Get(Asn.Uid));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


