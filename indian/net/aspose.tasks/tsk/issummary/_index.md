---
title: "Tsk.IsSummary"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk field. निर्धारित करता है कि क्या कार्य एक सारांश कार्य है"
type: docs
weight: 720
url: /hi/net/aspose.tasks/tsk/issummary/
---
## Tsk.IsSummary field

निर्धारित करता है कि कार्य एक सारांश कार्य है या नहीं।

```csharp
public static readonly Key<bool, TaskKey> IsSummary;
```

## उदाहरण

दिखाता है कि कैसे Tsk.IsSummary प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSummary, true);

Console.WriteLine("Is Summary: " + task.Get(Tsk.IsSummary));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


