---
title: "Tsk.IsExpanded"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। GanttChart दृश्य में यह निर्धारित करता है कि सारांश कार्य विस्तारित है या नहीं"
type: docs
weight: 590
url: /hi/net/aspose.tasks/tsk/isexpanded/
---
## Tsk.IsExpanded field

निर्धारित करता है कि GanttChart दृश्य में सारांश कार्य विस्तारित है या नहीं।

```csharp
public static readonly Key<NullableBool, TaskKey> IsExpanded;
```

## उदाहरण

दिखाता है कि कैसे Tsk.IsExpanded प्रॉपर्टी को पढ़ा/लिखा जाए।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsExpanded, true);

Console.WriteLine("Is Expanded: " + task.Get(Tsk.IsExpanded));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


