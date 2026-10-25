---
title: "Tsk.Contact"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. اسم الفرد المسؤول عن المهمة"
type: docs
weight: 220
url: /ar/net/aspose.tasks/tsk/contact/
---
## Tsk.Contact field

اسم الفرد المسؤول عن المهمة.

```csharp
public static readonly Key<string, TaskKey> Contact;
```

## الأمثلة

يظهر كيفية قراءة/كتابة خاصية Tsk.Contact.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Contact, "John Smith");

Console.WriteLine("Contact: " + task.Get(Tsk.Contact));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


