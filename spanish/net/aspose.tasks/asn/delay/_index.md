---
title: "Asn.Delay"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. El retraso de una asignación"
type: docs
weight: 230
url: /es/net/aspose.tasks/asn/delay/
---
## Asn.Delay field

El retraso de una asignación.

```csharp
public static readonly Key<Duration, AsnKey> Delay;
```

## Ejemplos

Muestra cómo leer/escribir las propiedades Asn.Delay y Asn.LevelingDelay.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Delay, project.GetDuration(0, TimeUnitType.Day));

Console.WriteLine("Delay: " + assignment.Get(Asn.Delay));
Console.WriteLine("Leveling Delay: " + assignment.Get(Asn.LevelingDelay));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


