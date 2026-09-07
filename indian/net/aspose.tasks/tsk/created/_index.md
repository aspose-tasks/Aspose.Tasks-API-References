---
title: "Tsk.Created"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। वह तिथि जब कार्य बनाया गया था"
type: docs
weight: 250
url: /hi/net/aspose.tasks/tsk/created/
---
## Tsk.Created field

कार्य के निर्मित होने की तिथि।

```csharp
public static readonly Key<DateTime, TaskKey> Created;
```

## उदाहरण

दिखाता है कि Tsk.Created प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + task.Get(Tsk.Created));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


