---
title: "Tsk.IsRecurring"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। यह निर्धारित करता है कि कार्य आवर्ती कार्यों की श्रृंखला का हिस्सा है या नहीं"
type: docs
weight: 670
url: /hi/net/aspose.tasks/tsk/isrecurring/
---
## Tsk.IsRecurring field

निर्धारित करता है कि कार्य आवर्ती कार्यों की श्रृंखला का हिस्सा है या नहीं।

```csharp
public static readonly Key<NullableBool, TaskKey> IsRecurring;
```

## उदाहरण

दिखाता है कि Tsk.IsRecurring प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRecurring, true);

Console.WriteLine("Is Recurring: " + task.Get(Tsk.IsRecurring));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


