---
title: "TaskBaseline.GetHashCode"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة TaskBaseline. تُرجع قيمة رمز تجزئة للمثيل من فئة TaskBaseline"
type: docs
weight: 110
url: /ar/net/aspose.tasks/taskbaseline/gethashcode/
---
## TaskBaseline.GetHashCode method

تُرجع قيمة رمز تجزئة للمثيل من الفئة [`TaskBaseline`](../).

```csharp
public override int GetHashCode()
```

### قيمة الإرجاع

تُرجع قيمة رمز تجزئة لهذا الكائن.

## الأمثلة

يظهر كيفية الحصول على رمز تجزئة لخط أساس المهمة.

```csharp
var project = new Project();

// إنشاء TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// عرض مدة TaskBaseline للمهمة
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// رمز التجزئة للتقويم يساوي رقم خط الأساس
Console.WriteLine("Baseline 1 Number: {0} Hash Code: {1}", (int)baseline1.BaselineNumber, baseline1.GetHashCode());
Console.WriteLine("Baseline 2 Number: {0} Hash Code: {1}", (int)baseline2.BaselineNumber, baseline2.GetHashCode());
```

### انظر أيضًا

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


