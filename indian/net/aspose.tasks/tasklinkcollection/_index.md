---
title: "क्लास TaskLinkCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.TaskLinkCollection क्लास। टास्क ऑब्जेक्ट्स का संग्रह दर्शाता है"
type: docs
weight: 2420
url: /hi/net/aspose.tasks/tasklinkcollection/
---
## TaskLinkCollection class

[`Task`](../task/) ऑब्जेक्ट्स का संग्रह दर्शाता है।

```csharp
public class TaskLinkCollection : IList<TaskLink>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/tasklinkcollection/count/) { get; } | इस `TaskLinkCollection` ऑब्जेक्ट में मौजूद ऑब्जेक्ट्स की संख्या प्राप्त करता है। |
| [Item](../../aspose.tasks/tasklinkcollection/item/) { get; set; } | निर्दिष्ट सूचकांक पर तत्व को लौटाता है या सेट करता है। |
| [ParentProject](../../aspose.tasks/tasklinkcollection/parentproject/) { get; } | ResourceAssignmentCollection ऑब्जेक्ट के पैरेंट प्रोजेक्ट को प्राप्त करता है। इस ऑब्जेक्ट के लिए पैरेंट [`Project`](../project/)। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_3)(TaskLink) | यह ICollection की Add मेथड की स्टब इम्प्लीमेंटेशन है, जो केवल NotSupportedException फेंकती है। |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add)(Task, Task) | Finish-Start [`TaskLink`](../tasklink/) का एक इंस्टेंस लौटाता है जिसे TaskLinkCollection ऑब्जेक्ट में जोड़ा गया है। |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_1)(Task, Task, TaskLinkType) | [`TaskLink`](../tasklink/) का एक इंस्टेंस लौटाता है जिसे TaskLinkCollection ऑब्जेक्ट में जोड़ा गया है। |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_2)(Task, Task, TaskLinkType, Duration) | [`TaskLink`](../tasklink/) का एक इंस्टेंस लौटाता है जिसे TaskLinkCollection ऑब्जेक्ट में जोड़ा गया है। |
| [GetEnumerator](../../aspose.tasks/tasklinkcollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [Remove](../../aspose.tasks/tasklinkcollection/remove/)(TaskLink) | प्रोजेक्ट से टास्क लिंक हटाता है। |
| [ToList](../../aspose.tasks/tasklinkcollection/tolist/)() | TaskLinkCollection ऑब्जेक्ट को [`TaskLink`](../tasklink/) ऑब्जेक्ट्स की सूची में परिवर्तित करता है। |

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

* class [TaskLink](../tasklink/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


