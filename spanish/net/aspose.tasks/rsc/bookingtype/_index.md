---
title: "Rsc.BookingType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Rsc campo. El tipo de reserva de un recurso"
type: docs
weight: 160
url: /es/net/aspose.tasks/rsc/bookingtype/
---
## Rsc.BookingType field

El tipo de reserva de un recurso.

```csharp
public static readonly Key<BookingType, RscKey> BookingType;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.BookingType.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.BookingType, BookingType.Committed);

Console.WriteLine("Booking Type: " + resource.Get(Rsc.BookingType));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BookingType](../../bookingtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


