---
title: "Asn.BookingType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. El tipo de reserva de una asignación"
type: docs
weight: 140
url: /es/net/aspose.tasks/asn/bookingtype/
---
## Asn.BookingType field

El tipo de reserva de una asignación.

```csharp
public static readonly Key<BookingType, AsnKey> BookingType;
```

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

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BookingType](../../bookingtype/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


