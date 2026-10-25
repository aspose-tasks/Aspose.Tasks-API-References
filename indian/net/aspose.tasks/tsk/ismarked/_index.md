---
title: "Tsk.IsMarked"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। दिखाता है कि कोई कार्य आगे की कार्रवाई या किसी प्रकार की पहचान के लिए चिह्नित है या नहीं"
type: docs
weight: 620
url: /hi/net/aspose.tasks/tsk/ismarked/
---
## Tsk.IsMarked field

दिखाता है कि कार्य को आगे की कार्रवाई या किसी प्रकार की पहचान के लिए चिह्नित किया गया है या नहीं।

```csharp
public static readonly Key<bool, TaskKey> IsMarked;
```

## टिप्पणियाँ

केवल mpp फ़ाइल स्वरूप पर लागू होता है।

## उदाहरण

दिखाता है कि कैसे Tsk.IsMarked प्रॉपर्टी को पढ़ा/लिखा जाए।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsMarked, true);

Console.WriteLine("Is Marked: " + task.Get(Tsk.IsMarked));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


