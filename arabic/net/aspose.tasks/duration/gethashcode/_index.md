---
title: "Duration.GetHashCode"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Duration. تُعيد قيمة رمز تجزئة لهذا الكائن"
type: docs
weight: 90
url: /ar/net/aspose.tasks/duration/gethashcode/
---
## Duration.GetHashCode method

يعيد قيمة رمز التجزئة لهذا الكائن.

```csharp
public override int GetHashCode()
```

### قيمة الإرجاع

يعيد قيمة رمز تجزئة لهذه النسخة من المدة.

## الأمثلة

يظهر كيفية الحصول على رمز تجزئة لمدّة.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// رمز تجزئة التقويم يعتمد على نوع وحدة الوقت والقيمة الأولية للمدة
// لذا رموز التجزئة التالية متساوية
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 2 Hash Code: {0}", duration2.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration2.GetHashCode()));

// لكن رموز التجزئة للمدة 1 و 3 ليست كذلك
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 3 Hash Code: {0}", duration3.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration3.GetHashCode()));
```

### انظر أيضًا

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


