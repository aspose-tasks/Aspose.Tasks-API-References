---
title: "Tsk.PreleveledFinish"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। वह समाप्ति तिथि जो कार्य की थी जब संसाधन स्तरन किया गया था"
type: docs
weight: 910
url: /hi/net/aspose.tasks/tsk/preleveledfinish/
---
## Tsk.PreleveledFinish field

संसाधन लेवलिंग करने से पहले कार्य की समाप्ति तिथि।

```csharp
public static readonly Key<DateTime, TaskKey> PreleveledFinish;
```

## उदाहरण

दिखाता है कि Tsk.PreleveledFinish प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PreleveledFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Preleveled Finish: " + task.Get(Tsk.PreleveledFinish));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


