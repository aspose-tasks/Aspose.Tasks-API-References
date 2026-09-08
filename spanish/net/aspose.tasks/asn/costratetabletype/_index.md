---
title: "Asn.CostRateTableType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. La tabla de tarifas de costo utilizada para esta asignación"
type: docs
weight: 190
url: /es/net/aspose.tasks/asn/costratetabletype/
---
## Asn.CostRateTableType field

La tabla de tarifas de costos utilizada para esta asignación.

```csharp
public static readonly Key<RateType, AsnKey> CostRateTableType;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Asn.CostRateTableType.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.CostRateTableType, RateType.B);

Console.WriteLine("Cost Rate Table Type: " + assignment.Get(Asn.CostRateTableType));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateType](../../ratetype/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


