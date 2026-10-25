---
title: "Prj.StatusDate"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। प्रगति दिखाने या अर्जित मूल्य कुल की गणना करने के लिए स्टेटस डेट। स्टेटस डेट वर्तमान तिथि (आज की तिथि) के समान होती है जब तक कि कोई अलग स्टेटस डेट निर्दिष्ट न किया गया हो।"
type: docs
weight: 690
url: /hi/net/aspose.tasks/prj/statusdate/
---
## Prj.StatusDate field

प्रगति दिखाने या अर्जित मूल्य कुल की गणना करने के लिए स्थिति तिथि। स्थिति तिथि वर्तमान तिथि (आज की तिथि) के समान होती है, जब तक कि कोई अलग स्थिति तिथि निर्दिष्ट न की गई हो।

```csharp
public static readonly Key<DateTime, PrjKey> StatusDate;
```

## उदाहरण

दिखाता है कि Prj.StatusDate प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.StatusDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Status Date: " + project.Get(Prj.StatusDate));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


