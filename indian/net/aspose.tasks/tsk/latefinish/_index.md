---
title: "Tsk.LateFinish"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk field. वह नवीनतम तिथि जिस पर कार्य परियोजना के समाप्ति को विलंबित किए बिना समाप्त हो सकता है"
type: docs
weight: 730
url: /hi/net/aspose.tasks/tsk/latefinish/
---
## Tsk.LateFinish field

परियोजना की समाप्ति को विलंब किए बिना किसी कार्य के समाप्त होने की सबसे अंतिम तिथि।

```csharp
public static readonly Key<DateTime, TaskKey> LateFinish;
```

## उदाहरण

दिखाता है कि कैसे Tsk.LateFinish प्रॉपर्टी को पढ़ा/लिखा जाए।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LateFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Late Finish: " + task.Get(Tsk.LateFinish));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


