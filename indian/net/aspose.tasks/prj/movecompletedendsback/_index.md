---
title: "Prj.MoveCompletedEndsBack"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। निर्धारित करता है कि स्थिति तिथि के बाद शुरू होने वाले कार्यों के पूर्ण भागों के अंत, जो पहले शुरू हुए थे, को स्थिति तिथि पर वापस ले जाना चाहिए या नहीं"
type: docs
weight: 490
url: /hi/net/aspose.tasks/prj/movecompletedendsback/
---
## Prj.MoveCompletedEndsBack field

निर्धारित करता है कि स्थिति तिथि के बाद शुरू होने के लिए निर्धारित कार्यों के पूर्ण भागों का अंत, जो पहले शुरू हो गए हैं, को स्थिति तिथि पर वापस ले जाना चाहिए या नहीं।

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsBack;
```

## उदाहरण

दिखाता है कि Prj.MoveCompletedEndsBack प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsBack, true);

Console.WriteLine("Move Completed Ends Back: " + project.Get(Prj.MoveCompletedEndsBack));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


