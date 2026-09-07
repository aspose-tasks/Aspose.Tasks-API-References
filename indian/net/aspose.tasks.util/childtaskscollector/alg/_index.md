---
title: "ChildTasksCollector.Alg"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ChildTasksCollector method. निर्दिष्ट वस्तु को प्रक्रिया करता है।"
type: docs
weight: 30
url: /hi/net/aspose.tasks.util/childtaskscollector/alg/
---
## ChildTasksCollector.Alg method

निर्दिष्ट ऑब्जेक्ट को प्रोसेस करता है।

```csharp
public override void Alg(Task el, int level)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| el | कार्य | प्रक्रिया करने के लिए वस्तु। |
| स्तर | Int32 | पेड़ नोड का स्तर। |

## उदाहरण

दिखाता है कि प्रोजेक्ट में सभी टास्क को एक साधारण सूची के रूप में कैसे इटरेट करें।

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// सभी एकत्रित कार्यों को पार्स करें
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### संबंधित देखें

* class [Task](../../../aspose.tasks/task/)
* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


