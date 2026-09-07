---
title: "Prj.CustomDateFormat"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। प्रोजेक्ट व्यू कस्टम डेट फ़ॉर्मेट। जब DateFormat प्रॉपर्टी को कस्टम पर सेट किया जाता है तो तिथियों को फ़ॉर्मेट करने के लिए उपयोग किया जाता है।"
type: docs
weight: 200
url: /hi/net/aspose.tasks/prj/customdateformat/
---
## Prj.CustomDateFormat field

प्रोजेक्ट व्यू कस्टम डेट फ़ॉर्मेट। जब [`DateFormat`](../dateformat/) प्रॉपर्टी को कस्टम पर सेट किया जाता है तो तिथियों को फ़ॉर्मेट करने के लिए उपयोग किया जाता है।

```csharp
public static readonly Key<string, PrjKey> CustomDateFormat;
```

## उदाहरण

दिखाता है कि Prj.CustomDateFormat प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.CustomDateFormat, "dd MMMM yyyy H:mm");

Console.WriteLine("Custom Date Format: " + project.Get(Prj.CustomDateFormat));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


