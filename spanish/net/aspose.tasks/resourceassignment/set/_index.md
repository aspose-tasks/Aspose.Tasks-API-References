---
title: "ResourceAssignment.Set"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ResourceAssignment. Mapea la propiedad especificada al valor especificado en este contenedor"
type: docs
weight: 750
url: /es/net/aspose.tasks/resourceassignment/set/
---
## ResourceAssignment.Set&lt;T&gt; method

Mapea la propiedad especificada al valor especificado en este contenedor.

```csharp
public void Set<T>(Key<T, AsnKey> key, T val)
```

| Parámetro | Descripción |
| --- | --- |
| T | el tipo del valor asignado. |
| key | la clave de propiedad especificada. [`Asn`](../../asn/) para obtener la clave de propiedad. |
| valor | el valor. |

## Ejemplos

Muestra cómo crear una asignación y obtener/establecer propiedades comunes de la asignación.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 2, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1));
task.Set(Tsk.Finish, new DateTime(2020, 4, 2, 17, 0, 0));
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);
resourceAssignment.Set(Asn.Start, new DateTime(2020, 4, 2, 8, 0, 0));
resourceAssignment.Set(Asn.Work, project.GetWork(1));
resourceAssignment.Set(Asn.Finish, new DateTime(2020, 4, 2, 17, 0, 0));

Console.WriteLine(resourceAssignment.Get(Asn.Start));
Console.WriteLine(resourceAssignment.Get(Asn.Work));
Console.WriteLine(resourceAssignment.Get(Asn.Finish));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


