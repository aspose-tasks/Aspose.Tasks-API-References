---
title: "Tsk.IsManual"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk field. निर्धारित करता है कि क्या कार्य मैन्युअल रूप से निर्धारित है"
type: docs
weight: 610
url: /hi/net/aspose.tasks/tsk/ismanual/
---
## Tsk.IsManual field

निर्धारित करता है कि कार्य मैन्युअल रूप से शेड्यूल किया गया है या नहीं।

```csharp
public static readonly Key<NullableBool, TaskKey> IsManual;
```

## उदाहरण

दिखाता है कि कैसे Tsk.IsManual प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsManual, true);

Console.WriteLine("Is Manual: " + task.Get(Tsk.IsManual));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


