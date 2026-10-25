---
title: "Tsk.ExternalUid"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحتوي على المعرف الفريد للمهام الخارجية عندما تكون المهمة خارجية"
type: docs
weight: 380
url: /ar/net/aspose.tasks/tsk/externaluid/
---
## Tsk.ExternalUid field

يحتوي على المعرف الفريد للمهمة الخارجية عندما تكون المهمة خارجية.

```csharp
public static readonly Key<int, TaskKey> ExternalUid;
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

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


