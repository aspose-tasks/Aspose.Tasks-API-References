---
title: "WorkingTime.Equals"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة WorkingTime. تتحقق من أن الكائنات متساوية"
type: docs
weight: 40
url: /ar/net/aspose.tasks/workingtime/equals/
---
## WorkingTime.Equals method

يتحقق من أن الكائنات متساوية.

```csharp
public override bool Equals(object obj)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| obj | كائن | الكائن الثاني للمقارنة. |

### قيمة الإرجاع

صحيح إذا كانت الكائنات متساوية، خطأ خلاف ذلك.

## الأمثلة

يعرض كيفية التحقق من مساواة وقت العمل.

```csharp
var workingTime1 = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 17);

// يتم التحقق من مساواة التقويمات مقابل تواريخ from و to لوقت العمل.
Console.WriteLine("Working Time 1 (From): " + workingTime1.From);
Console.WriteLine("Working Time 1 (To): " + workingTime1.To);

Console.WriteLine("Working Time 2 (From): " + workingTime2.From);
Console.WriteLine("Working Time 2 (To): " + workingTime2.To);
Console.WriteLine("Are working times equal: " + workingTime1.Equals(workingTime2));
```

### انظر أيضًا

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)


