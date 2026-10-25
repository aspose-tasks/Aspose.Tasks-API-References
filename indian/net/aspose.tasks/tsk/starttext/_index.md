---
title: "Tsk.StartText"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। कार्य की प्रारंभिक टेक्स्ट लौटाता है"
type: docs
weight: 1030
url: /hi/net/aspose.tasks/tsk/starttext/
---
## Tsk.StartText field

कार्य की प्रारम्भिक पाठ लौटाता है।

```csharp
public static readonly Key<string, TaskKey> StartText;
```

## उदाहरण

दिखाता है कि Tsk.StartText प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartText, "Start Task Text");

Console.WriteLine("Start Text: " + task.Get(Tsk.StartText));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


