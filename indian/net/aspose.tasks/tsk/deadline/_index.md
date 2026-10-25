---
title: "Tsk.Deadline"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। एक लक्ष्य तिथि जो दर्शाती है कि कार्य कब पूरा होना चाहिए"
type: docs
weight: 270
url: /hi/net/aspose.tasks/tsk/deadline/
---
## Tsk.Deadline field

एक लक्ष्य तिथि जो दर्शाती है कि कार्य कब पूरा होना चाहिए।

```csharp
public static readonly Key<DateTime, TaskKey> Deadline;
```

## उदाहरण

दिखाता है कि Tsk.Deadline प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Deadline, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Deadline: " + task.Get(Tsk.Deadline));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


