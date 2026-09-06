---
title: "TaskLink.IsCrossProject"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية TaskLink. تحصل أو تعين قيمة تشير إلى ما إذا كان السلف جزءًا من مشروع آخر"
type: docs
weight: 20
url: /ar/net/aspose.tasks/tasklink/iscrossproject/
---
## TaskLink.IsCrossProject property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان السلف جزءًا من مشروع آخر.

```csharp
public bool IsCrossProject { get; set; }
```

## الأمثلة

يوضح كيفية العثور على روابط مهام عبر المشاريع.

```csharp
var project = new Project(DataDir + "GetCrossProjectTaskLinks.mpp");

// تحقق من روابط مهام عبر المشاريع
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Task Link: " + taskLink.ToString());
    if (taskLink.IsCrossProject)
    {
        Console.WriteLine(taskLink.CrossProjectName);
    }
}
```

يوضح كيفية إنشاء رابط مهمة عبر المشروع - رابط إلى مهمة في مشروع آخر (خارجي).

```csharp
Project project = new Project();
var summary = project.RootTask.Children.Add("Summary Task");

// من أجل إنشاء رابط إلى مهمة من مشروع آخر يجب أن ننشئ
// نسختها (أو "خارجي") في المشروع الحالي.

Task t2 = summary.Children.Add("External Task");
t2.Set(Tsk.ExternalTaskProject, "ExternalProject.mpp"); // here we set path to external project's MPP file.
t2.Set(Tsk.ExternalId, 1); // Set External task's Id.
t2.Set(Tsk.ExternalUid, 2); // External task's Unique Id should be set.
t2.Set(Tsk.IsExternalTask, true);
t2.Set(Tsk.IsManual, new NullableBool(false));
t2.Set(Tsk.IsSummary, false);

Task t = summary.Children.Add("Task");
TaskLink link = project.TaskLinks.Add(t2, t);
link.IsCrossProject = true;
link.LinkType = TaskLinkType.FinishToStart;
link.CrossProjectName = "ExternalProject.mpp\\\\1"; // <- here external task's Id is used.
```

### انظر أيضًا

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


