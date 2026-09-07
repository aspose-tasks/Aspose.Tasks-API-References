---
title: "Prj.MoveCompletedEndsForward"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। निर्धारित करता है कि स्थिति तिथि से पहले पूर्ण होने वाले कार्यों के पूर्ण भागों का अंत, जो बाद में शुरू हुए थे, को स्थिति तिथि तक ले जाया जाना चाहिए या नहीं"
type: docs
weight: 500
url: /hi/net/aspose.tasks/prj/movecompletedendsforward/
---
## Prj.MoveCompletedEndsForward field

निर्धारित करता है कि स्थिति तिथि से पहले पूर्ण होने के लिए निर्धारित कार्यों के पूर्ण भागों का अंत, जो बाद में शुरू हुए हैं, को स्थिति तिथि तक ऊपर ले जाना चाहिए या नहीं।

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsForward;
```

## उदाहरण

दिखाता है कि Prj.MoveCompletedEndsForward प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsForward, true);

Console.WriteLine("Move Completed Ends Forward: " + project.Get(Prj.MoveCompletedEndsForward));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


