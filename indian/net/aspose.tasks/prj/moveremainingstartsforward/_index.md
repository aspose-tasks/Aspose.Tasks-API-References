---
title: "Prj.MoveRemainingStartsForward"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। निर्धारित करता है कि बाद में शुरू होने वाले शेड्यूल किए गए कार्यों के शेष भागों की शुरुआत को स्थिति तिथि तक आगे ले जाना चाहिए या नहीं"
type: docs
weight: 520
url: /hi/net/aspose.tasks/prj/moveremainingstartsforward/
---
## Prj.MoveRemainingStartsForward field

निर्धारित करता है कि क्या कार्यों के शेष भागों की शुरुआत, जो बाद में शुरू होने के लिए निर्धारित हैं, को स्थिति तिथि तक ऊपर ले जाया जाना चाहिए।

```csharp
public static readonly Key<NullableBool, PrjKey> MoveRemainingStartsForward;
```

## उदाहरण

दिखाता है कि Prj.MoveRemainingStartsForward प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.MoveRemainingStartsForward, true);

Console.WriteLine("Move Remaining Starts Forward: " + project.Get(Prj.MoveRemainingStartsForward));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


