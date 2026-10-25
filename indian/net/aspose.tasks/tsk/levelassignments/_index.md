---
title: "Tsk.LevelAssignments"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। निर्धारित करता है कि लेवलिंग फ़ंक्शन ओवर अलोकेशन को हल करने के लिए व्यक्तिगत असाइनमेंट को विलंबित और विभाजित कर सकता है या नहीं"
type: docs
weight: 750
url: /hi/net/aspose.tasks/tsk/levelassignments/
---
## Tsk.LevelAssignments field

निर्धारित करता है कि लेवलिंग फ़ंक्शन अधिक आवंटन को हल करने के लिए व्यक्तिगत असाइनमेंट को विलंब और विभाजित कर सकता है या नहीं।

```csharp
public static readonly Key<NullableBool, TaskKey> LevelAssignments;
```

## उदाहरण

दिखाता है कि कैसे Tsk.LevelAssignments प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelAssignments, true);

Console.WriteLine("Level Assignments: " + task.Get(Tsk.LevelAssignments));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


