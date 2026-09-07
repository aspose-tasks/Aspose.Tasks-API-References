---
title: "Prj.DateFormat"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। प्रोजेक्ट व्यू डेट फ़ॉर्मेट"
type: docs
weight: 210
url: /hi/net/aspose.tasks/prj/dateformat/
---
## Prj.DateFormat field

परियोजना दृश्य तिथि प्रारूप।

```csharp
public static readonly Key<DateFormat, PrjKey> DateFormat;
```

## उदाहरण

दिखाता है कि Prj.DateFormat प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.DateFormat, DateFormat.DateDd);

Console.WriteLine("Date Format: " + project.Get(Prj.DateFormat));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [DateFormat](../../dateformat/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


