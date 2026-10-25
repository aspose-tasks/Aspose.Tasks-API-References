---
title: "Task.ExternalId"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Task. يحصل أو يضبط قيمة ExternalId"
type: docs
weight: 410
url: /ar/net/aspose.tasks/task/externalid/
---
## Task.ExternalId property

يحصل أو يعيّن قيمة لـ ExternalId.

```csharp
public int ExternalId { get; set; }
```

## الأمثلة

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

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


