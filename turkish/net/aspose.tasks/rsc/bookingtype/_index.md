---
title: "Rsc.BookingType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynağın rezervasyon türü"
type: docs
weight: 160
url: /tr/net/aspose.tasks/rsc/bookingtype/
---
## Rsc.BookingType field

Bir kaynağın rezervasyon tipi.

```csharp
public static readonly Key<BookingType, RscKey> BookingType;
```

## Örnekler

Rsc.BookingType özelliğini okuma/yazma yöntemini gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.BookingType, BookingType.Committed);

Console.WriteLine("Booking Type: " + resource.Get(Rsc.BookingType));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BookingType](../../bookingtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


