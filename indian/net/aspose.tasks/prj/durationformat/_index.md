---
title: "Prj.DurationFormat"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। बल्क अवधि को व्यक्त करने का प्रारूप"
type: docs
weight: 300
url: /hi/net/aspose.tasks/prj/durationformat/
---
## Prj.DurationFormat field

समूह अवधि व्यक्त करने का प्रारूप।

```csharp
public static readonly Key<TimeUnitType, PrjKey> DurationFormat;
```

## उदाहरण

दिखाता है कि Prj.DurationFormat प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.DurationFormat, TimeUnitType.Day);

Console.WriteLine("Duration Format: " + project.Get(Prj.DurationFormat));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


