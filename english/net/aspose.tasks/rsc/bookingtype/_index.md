---
title: Rsc.BookingType
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The booking type of a resource
type: docs
weight: 160
url: /net/aspose.tasks/rsc/bookingtype/
---
## Rsc.BookingType field

The booking type of a resource.

```csharp
public static readonly Key<BookingType, RscKey> BookingType;
```

## Examples

Shows how to read/write Rsc.BookingType property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.BookingType, BookingType.Committed);

Console.WriteLine("Booking Type: " + resource.Get(Rsc.BookingType));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BookingType](../../bookingtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


