---
title: "Tsk.LateStart"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk field. वह नवीनतम तिथि जिस पर कोई कार्य परियोजना के समाप्ति को विलंबित किए बिना शुरू हो सकता है"
type: docs
weight: 740
url: /hi/net/aspose.tasks/tsk/latestart/
---
## Tsk.LateStart field

परियोजना की समाप्ति को विलंब किए बिना किसी कार्य के शुरू होने की सबसे अंतिम तिथि।

```csharp
public static readonly Key<DateTime, TaskKey> LateStart;
```

## उदाहरण

दिखाता है कि कैसे Tsk.LateStart प्रॉपर्टी को पढ़ा/लिखा जाए।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LateStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Late Start: " + task.Get(Tsk.LateStart));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


