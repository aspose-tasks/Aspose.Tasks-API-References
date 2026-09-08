---
title: "Rsc.BookingType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc field. Het boekingstype van een resource"
type: docs
weight: 160
url: /nl/net/aspose.tasks/rsc/bookingtype/
---
## Rsc.BookingType field

Het boekingstype van een resource.

```csharp
public static readonly Key<BookingType, RscKey> BookingType;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.BookingType te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.BookingType, BookingType.Committed);

Console.WriteLine("Booking Type: " + resource.Get(Rsc.BookingType));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BookingType](../../bookingtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


