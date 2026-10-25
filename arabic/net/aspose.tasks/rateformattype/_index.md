---
title: "التعداد RateFormatType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "التعداد Aspose.Tasks.RateFormatType. يحدد الوحدات التي يستخدمها Microsoft Project لعرض المعدل"
type: docs
weight: 1640
url: /ar/net/aspose.tasks/rateformattype/
---
## RateFormatType enumeration

يحدد الوحدات التي يستخدمها Microsoft Project لعرض المعدل.

```csharp
public enum RateFormatType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Undefined | `-1` | القيمة لم تُعرّف في ملف المشروع الأصلي. |
| Minute | `0` | دقيقة ("min") |
| Hour | `1` | ساعة ("hr") |
| Day | `2` | يوم ("day") |
| Week | `3` | أسبوع ("wk") |
| Month | `4` | شهر ("mo") |
| Year | `5` | سنة ("yr") |
| MaterialResourceRate | `6` | معدل مورد المادة (فارغ) |

## ملاحظات

أثناء التصدير إلى XML سيتم حذف القيم غير المعرفة من XML الناتج.

## الأمثلة

يوضح كيفية قراءة/كتابة الخاصية Rsc.StandardRateFormat.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.StandardRateFormat, RateFormatType.Hour);

Console.WriteLine("Standard Rate Format: " + resource.Get(Rsc.StandardRateFormat));
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


