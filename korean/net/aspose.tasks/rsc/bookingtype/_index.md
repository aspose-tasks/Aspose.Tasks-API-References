---
title: "Rsc.BookingType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스의 예약 유형"
type: docs
weight: 160
url: /ko/net/aspose.tasks/rsc/bookingtype/
---
## Rsc.BookingType field

리소스의 예약 유형.

```csharp
public static readonly Key<BookingType, RscKey> BookingType;
```

## 예제

Rsc.BookingType 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.BookingType, BookingType.Committed);

Console.WriteLine("Booking Type: " + resource.Get(Rsc.BookingType));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BookingType](../../bookingtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


