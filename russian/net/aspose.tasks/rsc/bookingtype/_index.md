---
title: "Rsc.BookingType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Тип бронирования ресурса"
type: docs
weight: 160
url: /ru/net/aspose.tasks/rsc/bookingtype/
---
## Rsc.BookingType field

Тип бронирования ресурса.

```csharp
public static readonly Key<BookingType, RscKey> BookingType;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.BookingType.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.BookingType, BookingType.Committed);

Console.WriteLine("Booking Type: " + resource.Get(Rsc.BookingType));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BookingType](../../bookingtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


