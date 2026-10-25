---
title: "Prj.MicrosoftProjectServerURL"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। निर्धारित करता है कि प्रोजेक्ट को Project Server उपयोगकर्ता द्वारा बनाया गया है या NT उपयोगकर्ता द्वारा।"
type: docs
weight: 460
url: /hi/net/aspose.tasks/prj/microsoftprojectserverurl/
---
## Prj.MicrosoftProjectServerURL field

निर्धारित करता है कि परियोजना Project Server उपयोगकर्ता द्वारा बनाई गई है या NT उपयोगकर्ता द्वारा।

```csharp
public static readonly Key<NullableBool, PrjKey> MicrosoftProjectServerURL;
```

## उदाहरण

दिखाता है कि Prj.MicrosoftProjectServerURL प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.MicrosoftProjectServerURL, true);

Console.WriteLine("Microsoft Project Server U R L: " + project.Get(Prj.MicrosoftProjectServerURL));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


