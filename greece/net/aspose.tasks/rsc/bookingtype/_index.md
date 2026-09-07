---
title: "Rsc.BookingType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Ο τύπος κράτησης ενός πόρου"
type: docs
weight: 160
url: /el/net/aspose.tasks/rsc/bookingtype/
---
## Rsc.BookingType field

Ο τύπος κράτησης ενός πόρου.

```csharp
public static readonly Key<BookingType, RscKey> BookingType;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.BookingType.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.BookingType, BookingType.Committed);

Console.WriteLine("Booking Type: " + resource.Get(Rsc.BookingType));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BookingType](../../bookingtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


