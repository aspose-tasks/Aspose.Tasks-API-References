---
title: "Tsk.DisplayOnTimeline"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। निर्दिष्ट करता है कि कार्य को टाइमलाइन दृश्य में दिखाया जाना चाहिए या नहीं"
type: docs
weight: 290
url: /hi/net/aspose.tasks/tsk/displayontimeline/
---
## Tsk.DisplayOnTimeline field

निर्दिष्ट करता है कि कार्य को टाइमलाइन दृश्य में दिखाया जाना चाहिए या नहीं।

```csharp
public static readonly Key<bool, TaskKey> DisplayOnTimeline;
```

## उदाहरण

दिखाता है कि Tsk.DisplayOnTimeline प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayOnTimeline, true);

Console.WriteLine("Display On Timeline: " + task.Get(Tsk.DisplayOnTimeline));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


