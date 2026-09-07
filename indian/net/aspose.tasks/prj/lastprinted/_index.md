---
title: "Prj.LastPrinted"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। प्रोजेक्ट का अंतिम प्रिंट समय। mpp फ़ाइलों में UTC प्रारूप में सहेजा गया। DateTime प्रकार"
type: docs
weight: 430
url: /hi/net/aspose.tasks/prj/lastprinted/
---
## Prj.LastPrinted field

परियोजना का अंतिम प्रिंट समय। mpp फ़ाइलों में UTC प्रारूप में सहेजा गया। DateTime प्रकार।

```csharp
public static readonly Key<DateTime, PrjKey> LastPrinted;
```

## उदाहरण

दिखाता है कि Prj.LastPrinted प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.LastPrinted, new DateTime(2020, 4, 10, 13, 0, 0));

Console.WriteLine("Last Printed: " + project.Get(Prj.LastPrinted));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


