---
title: "Tsk.EarlyStart"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। वह सबसे प्रारंभिक तिथि जब कार्य संभवतः शुरू हो सकता है, जो पूर्ववर्ती और उत्तराधिकारी कार्यों की प्रारंभ तिथियों और अन्य प्रतिबंधों पर आधारित है"
type: docs
weight: 340
url: /hi/net/aspose.tasks/tsk/earlystart/
---
## Tsk.EarlyStart field

पूर्ववर्ती और उत्तराधिकारी कार्यों की प्रारंभिक प्रारंभ तिथियों और अन्य प्रतिबंधों के आधार पर कार्य के शुरू होने की सबसे प्रारंभिक तिथि।

```csharp
public static readonly Key<DateTime, TaskKey> EarlyStart;
```

## उदाहरण

दिखाता है कि Tsk.EarlyStart प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Start: " + task.Get(Tsk.EarlyStart));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


