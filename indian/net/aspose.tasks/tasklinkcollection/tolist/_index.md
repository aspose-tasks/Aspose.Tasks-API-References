---
title: "TaskLinkCollection.ToList"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TaskLinkCollection मेथड। TaskLinkCollection ऑब्जेक्ट को TaskLink ऑब्जेक्ट्स की सूची में परिवर्तित करता है"
type: docs
weight: 70
url: /hi/net/aspose.tasks/tasklinkcollection/tolist/
---
## TaskLinkCollection.ToList method

TaskLinkCollection ऑब्जेक्ट को [`TaskLink`](../../tasklink/) ऑब्जेक्ट्स की सूची में परिवर्तित करता है।

```csharp
public List<TaskLink> ToList()
```

### रिटर्न वैल्यू

[`TaskLink`](../../tasklink/) ऑब्जेक्ट्स की सूची।

## उदाहरण

टास्क लिंक कलेक्शन्स के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// टास्क प्राप्त करें
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// टास्क को लिंक करें
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// टास्कों के बीच लिंक प्रिंट करें
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// इंडेक्स एक्सेस द्वारा लिंक संपादित करें
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// सभी टास्क लिंक हटाएँ
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### संबंधित देखें

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


