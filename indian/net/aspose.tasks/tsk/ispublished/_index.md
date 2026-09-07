---
title: "Tsk.IsPublished"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। निर्धारित करता है कि वर्तमान कार्य को प्रोजेक्ट सर्वर पर परियोजना के बाकी हिस्सों के साथ प्रकाशित किया जाना चाहिए या नहीं"
type: docs
weight: 660
url: /hi/net/aspose.tasks/tsk/ispublished/
---
## Tsk.IsPublished field

निर्धारित करता है कि वर्तमान कार्य को बाकी प्रोजेक्ट के साथ Project Server पर प्रकाशित किया जाना चाहिए या नहीं।

```csharp
public static readonly Key<NullableBool, TaskKey> IsPublished;
```

## उदाहरण

दिखाता है कि कैसे Tsk.IsPublished प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsPublished, true);

Console.WriteLine("Is Published: " + task.Get(Tsk.IsPublished));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


