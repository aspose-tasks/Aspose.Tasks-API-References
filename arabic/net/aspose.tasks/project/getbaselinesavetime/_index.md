---
title: "Project.GetBaselineSaveTime"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Project. تُرجع وقت حفظ الخط الأساسي"
type: docs
weight: 1090
url: /ar/net/aspose.tasks/project/getbaselinesavetime/
---
## Project.GetBaselineSaveTime method

يرجع وقت حفظ الخط الأساسي.

```csharp
public DateTime GetBaselineSaveTime(BaselineType baselineNumber)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| baselineNumber | BaselineType | رقم الخط الأساسي [`BaselineType`](../../baselinetype/). |

### قيمة الإرجاع

تاريخ ووقت الحفظ الأخير للخط الأساسي.

## ملاحظات

تُرجع DateTime.MinValue إذا لم يتم حفظ الخط الأساسي.

## الأمثلة

يظهر كيفية قراءة/كتابة وقت حفظ الخط الأساسي للمشروع.

```csharp
var project = new Project();
var baselineSave = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time before: " + baselineSave);

// تعيين وقت حفظ الخط الأساسي
project.SetBaselineSaveTime(BaselineType.Baseline, DateTime.Today);

var baselineSaveNew = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time after: " + baselineSaveNew);
```

### انظر أيضًا

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


