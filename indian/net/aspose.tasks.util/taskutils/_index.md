---
title: "क्लास TaskUtils"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Util.TaskUtils क्लास। एक हेल्पर क्लास जो टास्क्स के साथ उपयोगी ऑपरेशन्स प्रदान करता है"
type: docs
weight: 2770
url: /hi/net/aspose.tasks.util/taskutils/
---
## TaskUtils class

कार्य के साथ उपयोगी संचालन प्रदान करने वाली हेल्पर क्लास।

```csharp
public static class TaskUtils
```

## विधियाँ

| नाम | विवरण |
| --- | --- |
| static [Apply](../../aspose.tasks.util/taskutils/apply/)(Task, ITreeAlgorithm&lt;Task&gt;, int) | निर्दिष्ट एल्गोरिदम को ट्री के प्रत्येक टास्क पर लागू करता है। |
| static [Filter](../../aspose.tasks.util/taskutils/filter/)(Task, ICondition&lt;Task&gt;) | शर्त को पूरा करने वाले टास्क्स का नया ट्री बनाता है। |
| static [Find](../../aspose.tasks.util/taskutils/find/)(Task, ICondition&lt;Task&gt;) | टास्क्स के ट्री में शर्त को पूरा करने वाला टास्क खोजता है। |
| static [TaskChildrenCount](../../aspose.tasks.util/taskutils/taskchildrencount/)(Task) | सभी स्तरों पर पुनरावर्ती रूप से टास्क के चाइल्ड टास्क की संख्या की गणना करता है। |

## उदाहरण

ट्री एल्गोरिदम के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Project2.mpp");

// सभी प्रोजेक्ट टास्क इकट्ठा करें
var coll = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, coll, 0);

// टास्क्स को साधारण सूची की तरह काम करें
foreach (var task in coll.Tasks)
{
    Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
}
```

### संबंधित देखें

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


