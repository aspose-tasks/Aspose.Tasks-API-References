---
title: "Duration.Equals"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Duration. تُعيد قيمة تُشير إلى ما إذا كانت هذه النسخة مساوية لكائن محدد"
type: docs
weight: 80
url: /ar/net/aspose.tasks/duration/equals/
---
## Equals(Duration) {#equals}

يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد.

```csharp
public bool Equals(Duration other)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| آخر | المدة | الكائن للمقارنة مع هذه المثيلة. |

### قيمة الإرجاع

تُعيد **True** إذا كانت نسخة Duration الأخرى لديها نفس قيم TimeSpan و TimeUnit مثل هذه النسخة؛ وإلا، **false**.

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

---

## Equals(object) {#equals_1}

يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد.

```csharp
public override bool Equals(object obj)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| obj | كائن | الكائن للمقارنة مع هذه المثيلة. |

### قيمة الإرجاع

**True** if the specified object is a Duration that has the same TimeSpan and TimeUnit values as this instance; otherwise, **false**.

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


