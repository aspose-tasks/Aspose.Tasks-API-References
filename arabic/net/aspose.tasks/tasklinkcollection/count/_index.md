---
title: "TaskLinkCollection.Count"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية TaskLinkCollection. تحصل على عدد الكائنات الموجودة في كائن TaskLinkCollection هذا."
type: docs
weight: 10
url: /ar/net/aspose.tasks/tasklinkcollection/count/
---
## TaskLinkCollection.Count property

يحصل على عدد الكائنات الموجودة في كائن [`TaskLinkCollection`](../) هذا.

```csharp
public int Count { get; }
```

## الأمثلة

يوضح كيفية العمل مع مجموعات روابط المهام.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// احصل على المهام
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// اربط المهام
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// اطبع الروابط بين المهام
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// حرّر الرابط عبر الوصول بالفهرس
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// احذف جميع روابط المهام
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### انظر أيضًا

* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


