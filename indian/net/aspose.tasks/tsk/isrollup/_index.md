---
title: "Tsk.IsRollup"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। निर्धारित करता है कि उप‑कार्य Gantt बार की जानकारी सारांश कार्य बार में सम्मिलित होगी या नहीं"
type: docs
weight: 690
url: /hi/net/aspose.tasks/tsk/isrollup/
---
## Tsk.IsRollup field

निर्धारित करता है कि उपकार्य Gantt बार की जानकारी सारांश कार्य बार में सम्मिलित होगी या नहीं।

```csharp
public static readonly Key<NullableBool, TaskKey> IsRollup;
```

## उदाहरण

दिखाता है कि Tsk.IsRollup प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRollup, true);

Console.WriteLine("Is Rollup: " + task.Get(Tsk.IsRollup));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


