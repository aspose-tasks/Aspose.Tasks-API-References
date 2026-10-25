---
title: "Rsc.BookingType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. نوع الحجز للمورد"
type: docs
weight: 160
url: /ar/net/aspose.tasks/rsc/bookingtype/
---
## Rsc.BookingType field

نوع الحجز للمورد.

```csharp
public static readonly Key<BookingType, RscKey> BookingType;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Rsc.BookingType.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.BookingType, BookingType.Committed);

Console.WriteLine("Booking Type: " + resource.Get(Rsc.BookingType));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BookingType](../../bookingtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


