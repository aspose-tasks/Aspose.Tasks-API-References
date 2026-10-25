---
title: "Tsk.EarlyFinish"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड. पूर्ववर्ती और उत्तराधिकारी कार्यों की प्रारंभिक समाप्ति तिथियों, अन्य प्रतिबंधों और किसी भी लेवलिंग देरी के आधार पर कार्य के समाप्त होने की सबसे प्रारंभिक तिथि।"
type: docs
weight: 330
url: /hi/net/aspose.tasks/tsk/earlyfinish/
---
## Tsk.EarlyFinish field

पूर्ववर्ती और उत्तराधिकारी कार्यों की प्रारंभिक समाप्ति तिथियों, अन्य प्रतिबंधों और किसी भी लेवलिंग देरी के आधार पर कार्य के समाप्त होने की सबसे प्रारंभिक तिथि।

```csharp
public static readonly Key<DateTime, TaskKey> EarlyFinish;
```

## उदाहरण

Tsk.EarlyFinish प्रॉपर्टी को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Finish: " + task.Get(Tsk.EarlyFinish));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


