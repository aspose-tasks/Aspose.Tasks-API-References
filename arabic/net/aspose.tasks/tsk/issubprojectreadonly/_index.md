---
title: "Tsk.IsSubprojectReadOnly"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحدد ما إذا كان المشروع الفرعي للقراءة فقط"
type: docs
weight: 710
url: /ar/net/aspose.tasks/tsk/issubprojectreadonly/
---
## Tsk.IsSubprojectReadOnly field

يحدد ما إذا كان المشروع الفرعي للقراءة فقط.

```csharp
public static readonly Key<NullableBool, TaskKey> IsSubprojectReadOnly;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Tsk.IsSubprojectReadOnly.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSubprojectReadOnly, true);

Console.WriteLine("Is Subproject Read Only: " + task.Get(Tsk.IsSubprojectReadOnly));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


