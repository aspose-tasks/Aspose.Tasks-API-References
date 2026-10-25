---
title: "Prj.DefaultFinishTime"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. وقت الانتهاء الافتراضي للمهام الجديدة"
type: docs
weight: 230
url: /ar/net/aspose.tasks/prj/defaultfinishtime/
---
## Prj.DefaultFinishTime field

وقت الانتهاء الافتراضي للمهام الجديدة.

```csharp
public static readonly Key<DateTime, PrjKey> DefaultFinishTime;
```

## الأمثلة

يظهر كيفية قراءة/كتابة خاصية Prj.DefaultFinishTime.

```csharp
var project = new Project();

project.Set(Prj.DefaultFinishTime, new DateTime(2000, 1, 3, 10, 0, 0));

Console.WriteLine("Default Finish Time: " + project.Get(Prj.DefaultFinishTime));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


