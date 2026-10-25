---
title: "Prj.CriticalSlackLimit"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। यदि कुल स्लैक इस संख्या के दिनों से कम या बराबर हो तो MS Project द्वारा कार्यों को महत्वपूर्ण माना जाता है"
type: docs
weight: 140
url: /hi/net/aspose.tasks/prj/criticalslacklimit/
---
## Prj.CriticalSlackLimit field

यदि कुल स्लैक इस संख्या के दिनों से कम या बराबर है, तो MS Project द्वारा टास्क को क्रिटिकल माना जाता है।

```csharp
public static readonly Key<int, PrjKey> CriticalSlackLimit;
```

## उदाहरण

दिखाता है कि Prj.CriticalSlackLimit प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.CriticalSlackLimit, 2);

Console.WriteLine("Critical Slack Limit: " + project.Get(Prj.CriticalSlackLimit));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


