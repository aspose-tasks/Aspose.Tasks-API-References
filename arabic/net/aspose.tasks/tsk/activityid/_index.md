---
title: "Tsk.ActivityId"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يمثل حقل معرف النشاط، وهو معرف فريد للمهمة يستخدمه Primavera. ينطبق فقط على مشاريع Primavera."
type: docs
weight: 10
url: /ar/net/aspose.tasks/tsk/activityid/
---
## Tsk.ActivityId field

تمثل حقل معرف النشاط - المعرف الفريد للمهمة المستخدم في Primavera. (ينطبق فقط على مشاريع Primavera).

```csharp
public static readonly Key<string, TaskKey> ActivityId;
```

## الأمثلة

يوضح كيفية العمل مع حقل ActivityId الخاص بمشاريع Primavera.

```csharp
var project = new Project(DataDir + "test.xer");

var task = project.RootTask.Children.GetById(1);

Console.WriteLine("Task activity_id: {0}", task.Get(Tsk.ActivityId));

task.Set(Tsk.ActivityId, "CUSTOM_ACTIVITY_ID");

// إنشاء خيارات حفظ Primavera وتحديد أنه لا يجب استبدال معرفات ActivityIds أثناء الحفظ.
var options = new PrimaveraSaveOptions
{
    RenumberActivityIds = false
};

project.Save(OutDir + "WorkWithPrimaveraActivityId_out.xer", options);
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


