---
title: "TaskUtils.Apply"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TaskUtils मेथड। निर्दिष्ट एल्गोरिदम को पेड़ के प्रत्येक टास्क पर लागू करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks.util/taskutils/apply/
---
## TaskUtils.Apply method

निर्दिष्ट एल्गोरिदम को ट्री के प्रत्येक टास्क पर लागू करता है।

```csharp
public static void Apply(Task root, ITreeAlgorithm<Task> alg, int level)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| root | कार्य | पेड़ की जड़ |
| alg | ITreeAlgorithm`1 | लागू किया गया एल्गोरिदम। |
| स्तर | Int32 | जड़ टास्क का स्तर। |

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

* class [Task](../../../aspose.tasks/task/)
* interface [ITreeAlgorithm&lt;T&gt;](../../itreealgorithm-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


