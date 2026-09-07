---
title: "Rsc.BookingType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Il tipo di prenotazione di una risorsa"
type: docs
weight: 160
url: /it/net/aspose.tasks/rsc/bookingtype/
---
## Rsc.BookingType field

Il tipo di prenotazione di una risorsa.

```csharp
public static readonly Key<BookingType, RscKey> BookingType;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.BookingType.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.BookingType, BookingType.Committed);

Console.WriteLine("Booking Type: " + resource.Get(Rsc.BookingType));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BookingType](../../bookingtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


