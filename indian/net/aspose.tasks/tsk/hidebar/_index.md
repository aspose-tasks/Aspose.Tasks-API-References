---
title: "Tsk.HideBar"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। निर्धारित करता है कि Microsoft Project में प्रदर्शित होने पर कार्य की Gantt बार छिपी हुई है या नहीं"
type: docs
weight: 480
url: /hi/net/aspose.tasks/tsk/hidebar/
---
## Tsk.HideBar field

निर्धारित करता है कि Microsoft Project में प्रदर्शित होने पर कार्य की Gantt बार छिपी हुई है या नहीं।

```csharp
public static readonly Key<NullableBool, TaskKey> HideBar;
```

## उदाहरण

दिखाता है कि Tsk.HideBar प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.HideBar, true);

Console.WriteLine("Hide Bar: " + task.Get(Tsk.HideBar));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


