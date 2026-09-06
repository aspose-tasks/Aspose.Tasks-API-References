---
title: "Prj.CriticalSlackLimit"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. تُعتبر المهام حرجة في MS Project إذا كان إجمالي الفائض أقل أو يساوي هذا العدد من الأيام"
type: docs
weight: 140
url: /ar/net/aspose.tasks/prj/criticalslacklimit/
---
## Prj.CriticalSlackLimit field

تُعتبر المهام حرجة في MS Project إذا كان الفائض الكلي أقل أو يساوي هذا العدد من الأيام.

```csharp
public static readonly Key<int, PrjKey> CriticalSlackLimit;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Prj.CriticalSlackLimit.

```csharp
var project = new Project();

project.Set(Prj.CriticalSlackLimit, 2);

Console.WriteLine("Critical Slack Limit: " + project.Get(Prj.CriticalSlackLimit));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


