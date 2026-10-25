---
title: "Duration.op_Equality"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Duration. تُعيد قيمة تُشير إلى ما إذا كانت هذه النسخة مساوية لكائن محدد"
type: docs
weight: 140
url: /ar/net/aspose.tasks/duration/op_equality/
---
## Duration Equality operator

يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد.

```csharp
public static bool operator ==(Duration a, Duration b)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| a | المدة | المدة الأولى. |
| b | المدة | المدة الثانية. |

### قيمة الإرجاع

قيمة تشير إلى ما إذا كانت هذه النسخة مساوية لكائن محدد.

## الأمثلة

يظهر كيفية التحقق من مساواة المدة.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// يتم فحص مساواة المدة مقابل الفاصل الزمني الأساسي.
Console.WriteLine("Duration 1: " + duration1.TimeSpan);
Console.WriteLine("Duration 2: " + duration2.TimeSpan);
Console.WriteLine("Duration 3: " + duration3.TimeSpan);
Console.WriteLine("Are durations 1 and 2 equal: " + duration1.Equals(duration2));
Console.WriteLine("Are durations 1 and 3 equal: " + duration1.Equals(duration3));
```

### انظر أيضًا

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


