---
title: "Prj.MoveRemainingStartsBack"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। निर्धारित करता है कि स्थिति तिथि के बाद शुरू होने वाले लेकिन पहले शुरू हुए कार्यों के शेष भागों की शुरुआत को स्थिति तिथि पर वापस ले जाना चाहिए या नहीं।"
type: docs
weight: 510
url: /hi/net/aspose.tasks/prj/moveremainingstartsback/
---
## Prj.MoveRemainingStartsBack field

निर्धारित करता है कि क्या कार्यों के शेष भागों की शुरुआत, जो स्थिति तिथि के बाद शुरू होने के लिए निर्धारित हैं लेकिन पहले शुरू हो गए हैं, को स्थिति तिथि पर वापस ले जाया जाना चाहिए।

```csharp
public static readonly Key<NullableBool, PrjKey> MoveRemainingStartsBack;
```

## उदाहरण

दिखाता है कि Prj.MoveRemainingStartsBack प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.MoveRemainingStartsBack, true);

Console.WriteLine("Move Remaining Starts Back: " + project.Get(Prj.MoveRemainingStartsBack));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


