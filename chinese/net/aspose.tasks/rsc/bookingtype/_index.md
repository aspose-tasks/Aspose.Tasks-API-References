---
title: "Rsc.BookingType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。资源的预订类型"
type: docs
weight: 160
url: /zh/net/aspose.tasks/rsc/bookingtype/
---
## Rsc.BookingType field

资源的预订类型。

```csharp
public static readonly Key<BookingType, RscKey> BookingType;
```

## 示例

展示如何读取/写入 Rsc.BookingType 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.BookingType, BookingType.Committed);

Console.WriteLine("Booking Type: " + resource.Get(Rsc.BookingType));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BookingType](../../bookingtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


