---
title: "Tsk.PhysicalPercentComplete"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk field. पूर्णता प्रतिशत मान जिसे कार्य किए गए बजटेड लागत (BCWP) की गणना के वैकल्पिक रूप में उपयोग किया जा सकता है"
type: docs
weight: 900
url: /hi/net/aspose.tasks/tsk/physicalpercentcomplete/
---
## Tsk.PhysicalPercentComplete field

पूर्णता प्रतिशत मान जिसे कार्य किए गए बजटेड लागत (BCWP) की गणना के वैकल्पिक रूप में उपयोग किया जा सकता है।

```csharp
public static readonly Key<int, TaskKey> PhysicalPercentComplete;
```

## उदाहरण

दिखाता है कि कैसे Tsk.PhysicalPercentComplete प्रॉपर्टी को पढ़ा/लिखा जाए।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PhysicalPercentComplete, 10);

Console.WriteLine("Physical Percent Complete: " + task.Get(Tsk.PhysicalPercentComplete));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


