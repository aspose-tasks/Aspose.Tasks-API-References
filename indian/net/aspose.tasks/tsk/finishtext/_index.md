---
title: "Tsk.FinishText"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। कार्य का समाप्ति टेक्स्ट लौटाता है"
type: docs
weight: 410
url: /hi/net/aspose.tasks/tsk/finishtext/
---
## Tsk.FinishText field

कार्य की समाप्ति का पाठ लौटाता है।

```csharp
public static readonly Key<string, TaskKey> FinishText;
```

## उदाहरण

Tsk.FinishText प्रॉपर्टी को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishText, "Not A Finish");

Console.WriteLine("Finish Text: " + task.Get(Tsk.FinishText));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


