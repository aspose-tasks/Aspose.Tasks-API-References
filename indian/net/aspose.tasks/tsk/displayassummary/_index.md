---
title: "Tsk.DisplayAsSummary"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। यह निर्धारित करता है कि कार्य को सारांश कार्य के रूप में दिखाया जाना चाहिए या नहीं। पढ़ना केवल XML फ़ॉर्मेट के लिए समर्थित है"
type: docs
weight: 280
url: /hi/net/aspose.tasks/tsk/displayassummary/
---
## Tsk.DisplayAsSummary field

निर्धारित करता है कि कार्य को सारांश कार्य के रूप में दिखाया जाना चाहिए या नहीं। पढ़ना केवल XML प्रारूप के लिए समर्थित है।

```csharp
public static readonly Key<NullableBool, TaskKey> DisplayAsSummary;
```

## उदाहरण

दिखाता है कि Tsk.DisplayAsSummary प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayAsSummary, true);

Console.WriteLine("Display As Summary: " + task.Get(Tsk.DisplayAsSummary));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


