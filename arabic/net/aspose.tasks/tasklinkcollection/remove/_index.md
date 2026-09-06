---
title: "TaskLinkCollection.Remove"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة TaskLinkCollection. تزيل رابط المهمة من مشروع."
type: docs
weight: 60
url: /ar/net/aspose.tasks/tasklinkcollection/remove/
---
## TaskLinkCollection.Remove method

يزيل رابط المهمة من مشروع.

```csharp
public bool Remove(TaskLink item)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| العنصر | TaskLink | رابط المهمة المراد إزالته. |

### قيمة الإرجاع

تم إزالة رابط المهمة.

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

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


