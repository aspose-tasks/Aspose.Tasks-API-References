---
title: "Tsk.DurationText"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। कार्य की अवधि का टेक्स्ट लौटाता है"
type: docs
weight: 310
url: /hi/net/aspose.tasks/tsk/durationtext/
---
## Tsk.DurationText field

कार्य की अवधि का पाठ लौटाता है।

```csharp
public static readonly Key<string, TaskKey> DurationText;
```

## उदाहरण

दिखाता है कि Tsk.DurationText प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationText, "Not A Duration");

Console.WriteLine("Duration Text: " + task.Get(Tsk.DurationText));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


