---
title: "Tsk.StatusManager"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. اسم المورد المؤسسي الذي سيتلقى تحديثات الحالة للمهمة الحالية من الموارد"
type: docs
weight: 1050
url: /ar/net/aspose.tasks/tsk/statusmanager/
---
## Tsk.StatusManager field

اسم المورد المؤسسي الذي سيتلقى تحديثات الحالة للمهمة الحالية من الموارد.

```csharp
public static readonly Key<string, TaskKey> StatusManager;
```

## الأمثلة

يظهر كيفية قراءة/كتابة خاصية Tsk.StatusManager.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StatusManager, "John Smith");

Console.WriteLine("Status Manager: " + task.Get(Tsk.StatusManager));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


