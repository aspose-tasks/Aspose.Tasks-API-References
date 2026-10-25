---
title: "Asn.VAC"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. La diferencia entre el costo base y el costo total"
type: docs
weight: 590
url: /es/net/aspose.tasks/asn/vac/
---
## Asn.VAC field

La diferencia entre el costo de referencia y el costo total.

```csharp
public static readonly Key<double, AsnKey> VAC;
```

## Ejemplos

Muestra cómo leer la propiedad Asn.VAC.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.VAC, 10);

Console.WriteLine("VAC: " + assignment.Get(Asn.VAC));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


