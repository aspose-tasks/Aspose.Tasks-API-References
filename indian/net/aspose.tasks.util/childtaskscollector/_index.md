---
title: "क्लास ChildTasksCollector"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Util.ChildTasksCollector क्लास। सभी चाइल्ड टास्क एकत्र करता है।"
type: docs
weight: 2690
url: /hi/net/aspose.tasks.util/childtaskscollector/
---
## ChildTasksCollector class

सभी चाइल्ड कार्यों को एकत्र करता है।

```csharp
public class ChildTasksCollector : TreeAlgorithmBase<Task>
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [ChildTasksCollector](childtaskscollector/)() | `ChildTasksCollector` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Tasks](../../aspose.tasks.util/childtaskscollector/tasks/) { get; } | एकत्रित चाइल्ड ऑब्जेक्ट्स (टास्क) की सूची प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| override [Alg](../../aspose.tasks.util/childtaskscollector/alg/)(Task, int) | निर्दिष्ट ऑब्जेक्ट को प्रोसेस करता है। |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

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

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


