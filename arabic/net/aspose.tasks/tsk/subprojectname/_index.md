---
title: "Tsk.SubprojectName"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. موقع المصدر للمشروع الفرعي"
type: docs
weight: 1070
url: /ar/net/aspose.tasks/tsk/subprojectname/
---
## Tsk.SubprojectName field

موقع المصدر لمشروع فرعي.

```csharp
public static readonly Key<string, TaskKey> SubprojectName;
```

## الأمثلة

يعرض كيفية إنشاء مهمة مشروع فرعي.

```csharp
var project = new Project(DataDir + "SubProjectTask.mpp");

// إضافة مهمة
var task = project.RootTask.Children.Add("Task 1");

// إعداد رابط مشروع فرعي جديد
task.Set(Tsk.SubprojectName, DataDir + "subProject.mpp");

project.Save(OutDir + "CreateSubProjectTask_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


