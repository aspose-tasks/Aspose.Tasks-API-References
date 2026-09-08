---
title: "Asn.HasFixedRateUnits"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. Determina si las Unidades tienen tarifa fija"
type: docs
weight: 270
url: /es/net/aspose.tasks/asn/hasfixedrateunits/
---
## Asn.HasFixedRateUnits field

Determina si las Unidades tienen tarifa fija.

```csharp
public static readonly Key<bool, AsnKey> HasFixedRateUnits;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Asn.HasFixedRateUnits.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.HasFixedRateUnits, true);

Console.WriteLine("Has Fixed Rate Units: " + assignment.Get(Asn.HasFixedRateUnits));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


