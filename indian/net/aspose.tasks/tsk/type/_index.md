---
title: "Tsk.Type"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। कार्य का प्रकार"
type: docs
weight: 1100
url: /hi/net/aspose.tasks/tsk/type/
---
## Tsk.Type field

कार्य का प्रकार।

```csharp
public static readonly Key<TaskType, TaskKey> Type;
```

## उदाहरण

दिखाता है कि Tsk.Type प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Type, TaskType.FixedDuration);

Console.WriteLine("Type: " + task.Get(Tsk.Type));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskType](../../tasktype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


