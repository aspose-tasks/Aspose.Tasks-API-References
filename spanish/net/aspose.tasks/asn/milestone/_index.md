---
title: "Asn.Milestone"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. Determina si la asignación es un hito"
type: docs
weight: 330
url: /es/net/aspose.tasks/asn/milestone/
---
## Asn.Milestone field

Determina si la asignación es un hito.

```csharp
public static readonly Key<bool, AsnKey> Milestone;
```

## Ejemplos

Muestra cómo leer la propiedad Asn.Milestone.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Milestone: " + assignment.Get(Asn.Milestone));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


