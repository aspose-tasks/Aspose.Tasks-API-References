---
title: "Tsk.IsResumeValid"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk field. निर्धारित करता है कि क्या कार्य को पुनः शुरू किया जा सकता है"
type: docs
weight: 680
url: /hi/net/aspose.tasks/tsk/isresumevalid/
---
## Tsk.IsResumeValid field

निर्धारित करता है कि कार्य को पुनः शुरू किया जा सकता है या नहीं।

```csharp
public static readonly Key<NullableBool, TaskKey> IsResumeValid;
```

## उदाहरण

दिखाता है कि कैसे Tsk.IsResumeValid प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsResumeValid, true);

Console.WriteLine("Is Resume Valid: " + task.Get(Tsk.IsResumeValid));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


