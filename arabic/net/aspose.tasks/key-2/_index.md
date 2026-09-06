---
title: "بنية KeyTK"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "بنية Aspose.Tasks.Key2TK. تمثل مفتاح خاصية لفئة من النوع المحدد. يتم استخدام مثيل من هذه الفئة عند الحصول على خاصية أو تعيينها لحاوية."
type: docs
weight: 930
url: /ar/net/aspose.tasks/key-2/
---
## Key&lt;T,K&gt; structure

يمثل مفتاح خاصية لفئة من النوع المحدد. يتم استخدام نسخة من هذه الفئة عند الحصول على خاصية أو تعيينها لحاوية.

```csharp
public struct Key<T, K>
    where K : struct
```

| معامل | الوصف |
| --- | --- |
| T | نوع قيمة الخاصية. |
| K | نوع مفتاح الخاصية. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [KeyType](../../aspose.tasks/key-2/keytype/) { get; } | يحصل على مفتاح الخاصية. |

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Prj.ActualsInSync.

```csharp
var project = new Project();

project.Set(Prj.ActualsInSync, true);

Console.WriteLine("Actuals In Sync: " + project.Get(Prj.ActualsInSync));
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


