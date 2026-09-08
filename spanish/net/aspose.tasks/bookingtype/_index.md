---
title: "Enumeración BookingType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.BookingType. Especifica el tipo de reserva de un recurso."
type: docs
weight: 150
url: /es/net/aspose.tasks/bookingtype/
---
## BookingType enumeration

Especifica el tipo de reserva de un recurso.

```csharp
public enum BookingType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Undefined | `-1` | Indica que el valor no estaba definido en el archivo de proyecto original. |
| Committed | `0` | Indica el tipo de reserva comprometida. |
| Proposed | `1` | Indica el tipo de reserva propuesto. |

## Observaciones

Al exportar a XML, los valores Undefined se eliminarán del XML resultante.

## Ejemplos

Muestra cómo leer/escribir la propiedad Asn.BookingType.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.BookingType, BookingType.Proposed);

Console.WriteLine("Booking Type: " + assignment.Get(Asn.BookingType));
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


