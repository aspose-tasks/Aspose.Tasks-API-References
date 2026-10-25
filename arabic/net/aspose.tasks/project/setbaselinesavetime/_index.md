---
title: "Project.SetBaselineSaveTime"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Project. تعين وقت حفظ الخط الأساسي"
type: docs
weight: 1260
url: /ar/net/aspose.tasks/project/setbaselinesavetime/
---
## Project.SetBaselineSaveTime method

يضبط وقت حفظ الخط الأساسي.

```csharp
public void SetBaselineSaveTime(BaselineType baselineNumber, DateTime value)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| baselineNumber | BaselineType | رقم الخط الأساسي [`BaselineType`](../../baselinetype/). |
| value | DateTime | تاريخ ووقت الحفظ الأخير للخط الأساسي. |

## ملاحظات

عيّن القيمة إلى DateTime.MinValue إذا لم يتم حفظ الخط الأساسي.

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


