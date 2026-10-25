---
title: "Rsc.BookingType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Jenis pemesanan sebuah sumber daya"
type: docs
weight: 160
url: /id/net/aspose.tasks/rsc/bookingtype/
---
## Rsc.BookingType field

Jenis pemesanan sumber daya.

```csharp
public static readonly Key<BookingType, RscKey> BookingType;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.BookingType.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.BookingType, BookingType.Committed);

Console.WriteLine("Booking Type: " + resource.Get(Rsc.BookingType));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BookingType](../../bookingtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


