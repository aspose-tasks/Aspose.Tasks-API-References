---
title: "التعداد CurrencySymbolPositionType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "التعداد Aspose.Tasks.CurrencySymbolPositionType. يحدد موضع رمز العملة."
type: docs
weight: 370
url: /ar/net/aspose.tasks/currencysymbolpositiontype/
---
## CurrencySymbolPositionType enumeration

يحدد موضع رمز العملة.

```csharp
public enum CurrencySymbolPositionType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Undefined | `-1` | يشير إلى أن القيمة غير معرفة تعني أن الحقل لم يُعرّف في ملف المشروع الأصلي. |
| Before | `0` | يشير إلى نوع موضع الرمز قبل العملة. |
| After | `1` | يشير إلى نوع موضع الرمز بعد العملة. |
| BeforeWithSpace | `2` | يشير إلى نوع موضع الرمز قبل مع مسافة. |
| AfterWithSpace | `3` | يشير إلى نوع موضع الرمز بعد مع مسافة. |

## ملاحظات

أثناء التصدير إلى XML سيتم حذف القيم غير المعرفة من XML الناتج.

## الأمثلة

يظهر كيفية تحديد موضع رمز العملة (CurrencySymbolPositionType.Before).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// تعيين موضع رمز العملة
// قبل، بدون مسافة ($0).
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.Before);
// العمل مع المشروع...
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


