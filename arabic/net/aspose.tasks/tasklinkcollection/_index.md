---
title: "الفئة TaskLinkCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.TaskLinkCollection. تمثل مجموعة من كائنات Task"
type: docs
weight: 2420
url: /ar/net/aspose.tasks/tasklinkcollection/
---
## TaskLinkCollection class

تمثل مجموعة من كائنات [`Task`](../task/).

```csharp
public class TaskLinkCollection : IList<TaskLink>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/tasklinkcollection/count/) { get; } | يحصل على عدد الكائنات الموجودة في كائن `TaskLinkCollection` هذا. |
| [Item](../../aspose.tasks/tasklinkcollection/item/) { get; set; } | يرجع أو يعيّن العنصر في الفهرس المحدد. |
| [ParentProject](../../aspose.tasks/tasklinkcollection/parentproject/) { get; } | يحصل على المشروع الأب لكائن ResourceAssignmentCollection. المشروع الأب [`Project`](../project/) لهذا الكائن. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_3)(TaskLink) | هذا هو تنفيذ النموذج الأولي لطريقة Add في ICollection، والذي يرمي فقط NotSupportedException |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add)(Task, Task) | يعيد مثيلاً من Finish-Start [`TaskLink`](../tasklink/) الذي تم إضافته إلى كائن TaskLinkCollection. |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_1)(Task, Task, TaskLinkType) | يعيد مثيلاً من [`TaskLink`](../tasklink/) الذي تم إضافته إلى كائن TaskLinkCollection. |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_2)(Task, Task, TaskLinkType, Duration) | يعيد مثيلاً من [`TaskLink`](../tasklink/) الذي تم إضافته إلى كائن TaskLinkCollection. |
| [GetEnumerator](../../aspose.tasks/tasklinkcollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [Remove](../../aspose.tasks/tasklinkcollection/remove/)(TaskLink) | يزيل رابط المهمة من مشروع. |
| [ToList](../../aspose.tasks/tasklinkcollection/tolist/)() | يحوّل كائن TaskLinkCollection إلى قائمة من كائنات [`TaskLink`](../tasklink/). |

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

* class [TaskLink](../tasklink/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


