---
title: "Project.CriticalPath"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project प्रॉपर्टी। एक संग्रह प्राप्त करता है जिसमें इस प्रोजेक्ट के Critical Path को बनाते हुए Critical टास्क की सूची शामिल होती है। यह एक On ऑपरेशन है जहाँ n प्रोजेक्ट में टास्क की संख्या है।"
type: docs
weight: 180
url: /hi/net/aspose.tasks/project/criticalpath/
---
## Project.CriticalPath property

एक कलेक्शन प्राप्त करता है जिसमें इस प्रोजेक्ट के क्रिटिकल पाथ को बनाते हुए क्रिटिकल टास्क की सूची होती है। यह O(n) ऑपरेशन है, जहाँ n प्रोजेक्ट में टास्क की संख्या है।

```csharp
public TaskCollection CriticalPath { get; }
```

### रिटर्न वैल्यू

एक संग्रह जो सभी critical टास्क की सूची को दर्शाता है।

## उदाहरण

प्रोजेक्ट के critical path की गणना कैसे करें, यह दिखाता है।

```csharp
var project = new Project()
{
    CalculationMode = CalculationMode.Automatic
};

var subtask1 = project.RootTask.Children.Add("1");
var subtask2 = project.RootTask.Children.Add("2");
project.TaskLinks.Add(subtask1, subtask2, TaskLinkType.FinishToStart);

project.RootTask.Children.Add("3");

// अब critical path प्रदर्शित करें
foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id) + "  " + task.Get(Tsk.Name));
    Console.WriteLine(task.Get(Tsk.Start));
    Console.WriteLine(task.Get(Tsk.Finish) + "\n");
}
```

### संबंधित देखें

* class [TaskCollection](../../taskcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


