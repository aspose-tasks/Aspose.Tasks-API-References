---
title: "Rsc.BookingType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। किसी संसाधन का बुकिंग प्रकार"
type: docs
weight: 160
url: /hi/net/aspose.tasks/rsc/bookingtype/
---
## Rsc.BookingType field

संसाधन का बुकिंग प्रकार।

```csharp
public static readonly Key<BookingType, RscKey> BookingType;
```

## उदाहरण

दिखाता है कि कैसे Rsc.BookingType प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.BookingType, BookingType.Committed);

Console.WriteLine("Booking Type: " + resource.Get(Rsc.BookingType));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BookingType](../../bookingtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


