---
title: "Prj.ShowProjectSummaryTask"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। निर्धारित करता है कि गैंट चार्ट दृश्य के शीर्ष पर अपने स्वयं के सारांश कार्य बार के साथ पूरे प्रोजेक्ट की सारांश जानकारी को एक पंक्ति में दिखाया जाए या नहीं"
type: docs
weight: 640
url: /hi/net/aspose.tasks/prj/showprojectsummarytask/
---
## Prj.ShowProjectSummaryTask field

निर्धारित करता है कि क्या संपूर्ण परियोजना की सारांश जानकारी को एक पंक्ति में दिखाया जाए, जिसमें उसका अपना सारांश कार्य बार गैंट चार्ट दृश्य के शीर्ष पर हो।

```csharp
public static readonly Key<bool, PrjKey> ShowProjectSummaryTask;
```

## उदाहरण

दिखाता है कि Prj.ShowProjectSummaryTask प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.ShowProjectSummaryTask, true);

Console.WriteLine("Show Project Summary Task: " + project.Get(Prj.ShowProjectSummaryTask));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


