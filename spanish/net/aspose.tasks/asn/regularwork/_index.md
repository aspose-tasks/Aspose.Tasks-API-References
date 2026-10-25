---
title: "Asn.RegularWork"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. La cantidad de trabajo sin horas extra programado para una asignación"
type: docs
weight: 420
url: /es/net/aspose.tasks/asn/regularwork/
---
## Asn.RegularWork field

La cantidad de trabajo no extraordinario programado para una asignación.

```csharp
public static readonly Key<Duration, AsnKey> RegularWork;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Asn.RegularWork.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + assignment.Get(Asn.RegularWork));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


